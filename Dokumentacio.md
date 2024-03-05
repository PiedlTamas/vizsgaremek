# VIZSGAREMEK
### Budapesti Műszaki Szakképzési Centrum Neumann János Informatikai Technikum
### *Szakképesítés neve és száma:* Informatikai rendszer- és alkalmazás-üzemeltető technikus, 5-0612-12-02
### *Készítők neve, osztálya:* Piedl Tamás, Dobronay Péter; 2/14A
### Budapest, 2024.
### *A dolgozat címe:*
<br>

# [placeholder]

1. [VIZSGAREMEK](#vizsgaremek)
2. [\[placeholder\]](#placeholder)
    1. [Hálózati eszközök IP-címzése](#hálózati-eszközök-ip-címzése)
    2. [Területek IP-címtáblái:](#területek-ip-címtáblái)
        1. [HQ](#hq)
        2. [Raktár](#raktár)
        3. [Home Office](#home-office)
        4. [ISP](#isp)

## Hálózati eszközök IP-címzése

Az IP *(Internet Protocol)* címek megfelelő kezelése, kiosztása elengedhetetlen egy hálózatnál, legyen szó akár kis vagy nagy vállalkozásról, szervezetről. Azért, hogy hatékonyan tudjuk kiosztani a véges számú IP-címeket, VLSM-et *(Variable Length Subnet Mask)*, azaz változó hosszúságú alhálózati maszkot használunk, ami lehetőséget ad az hatékonyabb alhálózatokra bontásra, címkiosztásra. Az alhálózatokat úgy hoztuk létre, hogy ha a jövőben még szükség lenne plusz címekre, akkor beleférjenek a már meglévő hálózatokba, de figyelembe vettük, hogy melyik részeken várható esetleges bővítés.

## Területek IP-címtáblái:

### HQ

<table>
    <thead>
        <tr>
            <th colspan="2">Recepció</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>VLAN szám</td>
            <td>10</td>
        </tr>
        <tr>
            <td>Hálózati cím</td>
            <td>192.168.0.192</td>
        </tr>
        <tr>
            <td>Maszk (prefix);<br>
            összesen felhasználható címek</td>
            <td>255.255.255.240 (/28); 14 host</td>
        </tr>
        <tr>
            <td>Alapértelmezett átjáró</td>
            <td></td>
        </tr>
        <tr>
            <td>Beállított DNS-cím</td>
            <td>192.168.0.132</td>
        </tr>
        <tr>
            <td colspan="2"><i>Eszközök:</i></td>
        </tr>
        <tr>
            <td colspan="2"><u>PC0</u></td>
        </tr>
        <tr>
            <td><i>Interfész</i></td>
            <td><i>IP-cím</i></td>
        </tr>
        <tr>
            <td>FastEthernet0</td>
            <td>DHCP-től kapva</td>
        </tr>
        <tr>
            <td colspan="2"><u>PC1</u></td>
        </tr>
        <tr>
            <td><i>Interfész</i></td>
            <td><i>IP-cím</i></td>
        </tr>
        <tr>
            <td>FastEthernet0</td>
            <td>DHCP-től kapva</td>
        </tr>
        <tr>
            <td colspan="2"><u>Printer0</u></td>
        </tr>
        <tr>
            <td><i>Interfész</i></td>
            <td><i>IP-cím</i></td>
        </tr>
        <tr>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td colspan="2"><u>Laptop1</u></td>
        </tr>
        <tr>
            <td><i>Interfész</i></td>
            <td><i>IP-cím</i></td>
        </tr>
        <tr>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td colspan="2"><u>IP Phone0</u></td>
        </tr>
        <tr>
            <td><i>Interfész</i></td>
            <td><i>IP-cím</i></td>
        </tr>
        <tr>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td colspan="2"><u>TV0</u></td>
        </tr>
        <tr>
            <td><i>Interfész</i></td>
            <td><i>IP-cím</i></td>
        </tr>
        <tr>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td colspan="2"><u>Guest Wifi</u></td>
        </tr>
        <tr>
            <td><i>Interfész</i></td>
            <td><i>IP-cím</i></td>
        </tr>
        <tr>
            <td></td>
            <td></td>
        </tr>
    </tbody>
</table>


<table>
    <thead>
        <tr>
            <th colspan="2">Recepció Guest Wifi</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>VLAN szám</td>
            <td></td>
        </tr>
        <tr>
            <td>Hálózati cím</td>
            <td></td>
        </tr>
        <tr>
            <td>Maszk (prefix);<br>
            összesen felhasználható címek</td>
            <td>255.255.255.X (/Y); Z host</td>
        </tr>
        <tr>
            <td>Alapértelmezett átjáró</td>
            <td></td>
        </tr>
        <tr>
            <td>Beállított DNS-cím</td>
            <td></td>
        </tr>
        <tr>
            <td colspan="2"><i>Eszközök:</i></td>
        </tr>
        <tr>
            <td colspan="2"><u>Smartphone0</u></td>
        </tr>
        <tr>
            <td><i>Interfész</i></td>
            <td><i>IP-cím</i></td>
        </tr>
        <tr>
            <td></td>
            <td></td>
        </tr>
    </tbody>
</table>


<table>
    <thead>
        <tr>
            <th colspan="2">Iroda</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>VLAN szám</td>
            <td>20</td>
        </tr>
        <tr>
            <td>Hálózati cím</td>
            <td>192.168.0.0</td>
        </tr>
        <tr>
            <td>Maszk (prefix);<br>
            összesen felhasználható címek</td>
            <td>255.255.255.192 (/26); 62 host</td>
        </tr>
        <tr>
            <td>Alapértelmezett átjáró</td>
            <td></td>
        </tr>
        <tr>
            <td>Beállított DNS-cím</td>
            <td>192.168.0.132</td>
        </tr>
        <tr>
            <td colspan="2"><i>Eszközök:</i></td>
        </tr>
        <tr>
            <td colspan="2"><u>PC2</u></td>
        </tr>
        <tr>
            <td><i>Interfész</i></td>
            <td><i>IP-cím</i></td>
        </tr>
        <tr>
            <td>FastEthernet0</td>
            <td>DHCP-től kapva</td>
        </tr>
        <tr>
            <td colspan="2"><u>PC6</u></td>
        </tr>
        <tr>
            <td><i>Interfész</i></td>
            <td><i>IP-cím</i></td>
        </tr>
        <tr>
            <td>FastEthernet0</td>
            <td>DHCP-től kapva</td>
        </tr>
        <tr>
            <td colspan="2"><u>Printer1</u></td>
        </tr>
        <tr>
            <td><i>Interfész</i></td>
            <td><i>IP-cím</i></td>
        </tr>
        <tr>
            <td></td>
            <td></td>
        </tr>
    </tbody>
</table>


<table>
    <thead>
        <tr>
            <th colspan="2">Szoftverfejlesztők</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>VLAN szám</td>
            <td>30</td>
        </tr>
        <tr>
            <td>Hálózati cím</td>
            <td>192.168.0.64</td>
        </tr>
        <tr>
            <td>Maszk (prefix);<br>
            összesen felhasználható címek</td>
            <td>255.255.255.192 (/26); 62 host</td>
        </tr>
        <tr>
            <td>Alapértelmezett átjáró</td>
            <td></td>
        </tr>
        <tr>
            <td>Beállított DNS-cím</td>
            <td></td>
        </tr>
        <tr>
        <tr>
            <td colspan="2"><i>Eszközök:</i></td>
        </tr>
        <tr>
            <td colspan="2"><u>PC3</u></td>
        </tr>
        <tr>
            <td><i>Interfész</i></td>
            <td><i>IP-cím</i></td>
        </tr>
        <tr>
            <td>FastEthernet0</td>
            <td>DHCP-től kapva</td>
        </tr>
        <tr>
            <td colspan="2"><u>Printer2</u></td>
        </tr>
        <tr>
            <td><i>Interfész</i></td>
            <td><i>IP-cím</i></td>
        </tr>
        <tr>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td colspan="2"><u>Laptop2</u></td>
        </tr>
        <tr>
            <td><i>Interfész</i></td>
            <td><i>IP-cím</i></td>
        </tr>
        <tr>
            <td></td>
            <td></td>
        </tr>
    </tbody>
</table>


<table>
    <thead>
        <tr>
            <th colspan="2">Vezetőség és Tárgyalóterem</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>VLAN szám</td>
            <td>50</td>
        </tr>
        <tr>
            <td>Hálózati cím</td>
            <td>192.168.0.160</td>
        </tr>
        <tr>
            <td>Maszk (prefix);<br>
            összesen felhasználható címek</td>
            <td>255.255.255.224 (/27); 30 host</td>
        </tr>
        <tr>
            <td>Alapértelmezett átjáró</td>
            <td></td>
        </tr>
        <tr>
            <td>Beállított DNS-cím</td>
            <td></td>
        </tr>
        <tr>
            <td colspan="2"><i>Eszközök:</i></td>
        </tr>
        <tr>
            <td colspan="2"><u>PC5</u></td>
        </tr>
        <tr>
            <td><i>Interfész</i></td>
            <td><i>IP-cím</i></td>
        </tr>
        <tr>
            <td>FastEthernet0</td>
            <td>DHCP-től kapva</td>
        </tr>
        <tr>
            <td colspan="2"><u>Printer3</u></td>
        </tr>
        <tr>
            <td><i>Interfész</i></td>
            <td><i>IP-cím</i></td>
        </tr>
        <tr>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td colspan="2"><u>Laptop4</u></td>
        </tr>
        <tr>
            <td><i>Interfész</i></td>
            <td><i>IP-cím</i></td>
        </tr>
        <tr>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td colspan="2"><u>IP Phone1</u></td>
        </tr>
        <tr>
            <td><i>Interfész</i></td>
            <td><i>IP-cím</i></td>
        </tr>
        <tr>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td colspan="2"><u>TV1</u></td>
        </tr>
        <tr>
            <td><i>Interfész</i></td>
            <td><i>IP-cím</i></td>
        </tr>
        <tr>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td colspan="2"><u>Smartphone1</u></td>
        </tr>
        <tr>
            <td><i>Interfész</i></td>
            <td><i>IP-cím</i></td>
        </tr>
        <tr>
            <td></td>
            <td></td>
        </tr>
    </tbody>
</table>


<table>
    <thead>
        <tr>
            <th colspan="2">Rendszergazdák</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>VLAN szám</td>
            <td>-</td>
        </tr>
        <tr>
            <td>Hálózati cím</td>
            <td>192.168.0.208</td>
        </tr>
        <tr>
            <td>Maszk (prefix);<br>
            összesen felhasználható címek</td>
            <td>255.255.255.248 (/29); 6 host</td>
        </tr>
        <tr>
            <td>Alapértelmezett átjáró</td>
            <td></td>
        </tr>
        <tr>
            <td>Beállított DNS-cím</td>
            <td></td>
        </tr>
        <tr>
            <td colspan="2"><i>Eszközök:</i></td>
        </tr>
    </tbody>
</table>


<table>
    <thead>
        <tr>
            <th colspan="2">Szerverek</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>VLAN szám</td>
            <td>-</td>
        </tr>
        <tr>
            <td>Hálózati cím</td>
            <td>192.168.0.128</td>
        </tr>
        <tr>
            <td>Maszk (prefix);<br>
            összesen felhasználható címek</td>
            <td>255.255.255.240 (/28); 14 host</td>
        </tr>
        <tr>
            <td>Alapértelmezett átjáró</td>
            <td>192.168.0.129</td>
        </tr>
        <tr>
            <td>Beállított DNS-cím</td>
            <td>192.168.0.132</td>
        </tr>
        <tr>
            <td colspan="2"><i>Eszközök:</i></td>
        </tr>
        <tr>
            <td colspan="2"><u>DNS</u></td>
        </tr>
        <tr>
            <td><i>Interfész</i></td>
            <td><i>IP-cím</i></td>
        </tr>
        <tr>
            <td>FastEthernet0</td>
            <td>192.168.0.132</td>
        </tr>
        <tr>
            <td colspan="2"><u>FTP</u></td>
        </tr>
        <tr>
            <td><i>Interfész</i></td>
            <td><i>IP-cím</i></td>
        </tr>
        <tr>
            <td>FastEthernet0</td>
            <td>192.168.0.133</td>
        </tr>
        <tr>
            <td colspan="2"><u>WEB</u></td>
        </tr>
        <tr>
            <td><i>Interfész</i></td>
            <td><i>IP-cím</i></td>
        </tr>
        <tr>
            <td>FastEthernet0</td>
            <td>192.168.0.134</td>
        </tr>
        <tr>
            <td colspan="2"><u>LC</u></td>
        </tr>
        <tr>
            <td><i>Interfész</i></td>
            <td><i>IP-cím</i></td>
        </tr>
        <tr>
            <td>GigabitEthernet0</td>
            <td>192.168.0.135</td>
        </tr>
    </tbody>
</table>


<table>
    <thead>
        <tr>
            <th colspan="3">További eszközök</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td colspan="3"><u>Router17</u></td>
        </tr>
        <tr>
            <td><i>Interfész</i></td>
            <td><i>IP-cím</i></td>
            <td><i>Maszk</i></td>
        </tr>
        <tr>
            <td>GigabitEthernet4/0</td>
            <td>192.168.0.230</td>
            <td>255.255.255.252</td>
        </tr>
        <tr>
            <td>GigabitEthernet8/0.10</td>
            <td>192.168.0.193</td>
            <td>255.255.255.240</td>
        </tr>
        <tr>
            <td>GigabitEthernet8/0.20</td>
            <td>192.168.0.1</td>
            <td>255.255.255.192</td>
        </tr>
        <tr>
            <td>GigabitEthernet8/0.30</td>
            <td>192.168.0.65</td>
            <td>255.255.255.192</td>
        </tr>
        <tr>
            <td>GigabitEthernet8/0.50</td>
            <td>192.168.0.161</td>
            <td>255.255.255.224</td>
        </tr>
        <tr>
            <td>GigabitEthernet8/0.99</td>
            <td>192.168.0.145</td>
            <td>255.255.255.240</td>
        </tr>
        <tr>
            <td>GigabitEthernet9/0</td>
            <td>192.168.0.233</td>
            <td>255.255.255.252</td>
        </tr>
        <tr>
            <td colspan="3"><u>Router1</u></td>
        </tr>
        <tr>
            <td><i>Interfész</i></td>
            <td><i>IP-cím</i></td>
            <td><i>Maszk</i></td>
        </tr>
        <tr>
            <td>GigabitEthernet4/0</td>
            <td>192.168.0.229</td>
            <td>255.255.255.252</td>
        </tr>
        <tr>
            <td>GigabitEthernet5/0</td>
            <td>192.168.0.237</td>
            <td>255.255.255.252</td>
        </tr>
        <tr>
            <td>GigabitEthernet6/0</td>
            <td>192.168.0.226</td>
            <td>255.255.255.252</td>
        </tr>
        <tr>
            <td>GigabitEthernet7/0.10</td>
            <td>192.168.0.194</td>
            <td>255.255.255.240</td>
        </tr>
        <tr>
            <td>GigabitEthernet7/0.20</td>
            <td>192.168.0.2</td>
            <td>255.255.255.192</td>
        </tr>
        <tr>
            <td>GigabitEthernet7/0.30</td>
            <td>192.168.0.66</td>
            <td>255.255.255.192</td>
        </tr>
        <tr>
            <td>GigabitEthernet7/0.50</td>
            <td>192.168.0.162</td>
            <td>255.255.255.224</td>
        </tr>
        <tr>
            <td>GigabitEthernet7/0.99</td>
            <td>192.168.0.146</td>
            <td>255.255.255.240</td>
        </tr>
        <tr>
            <td>GigabitEthernet8/0</td>
            <td>192.168.0.129</td>
            <td>255.255.255.240</td>
        </tr>
        <tr>
            <td colspan="3"><u>HQEdge</u></td>
        </tr>
        <tr>
            <td><i>Interfész</i></td>
            <td><i>IP-cím</i></td>
            <td><i>Maszk</i></td>
        </tr>
        <tr>
            <td>Serial2/0</td>
            <td>192.168.0.221</td>
            <td>255.255.255.252</td>
        </tr>
        <tr>
            <td>GigabitEthernet4/0</td>
            <td>192.168.0.221</td>
            <td>255.255.255.252</td>
        </tr>
        <tr>
            <td>GigabitEthernet5/0</td>
            <td>192.168.0.225</td>
            <td>255.255.255.252</td>
        </tr>
        <tr>
            <td>GigabitEthernet9/0</td>
            <td>192.168.0.217</td>
            <td>255.255.255.252</td>
        </tr>
        <tr>
            <td colspan="3"><u>Router3</u></td>
        </tr>
        <tr>
            <td><i>Interfész</i></td>
            <td><i>IP-cím</i></td>
            <td><i>Maszk</i></td>
        </tr>
        <tr>
            <td>GigabitEthernet4/0</td>
            <td>192.168.0.238</td>
            <td>255.255.255.252</td>
        </tr>
        <tr>
            <td>GigabitEthernet5/0</td>
            <td>192.168.0.234</td>
            <td>255.255.255.252</td>
        </tr>
        <tr>
            <td>GigabitEthernet9/0</td>
            <td>192.168.0.193</td>
            <td>255.255.255.248</td>
        </tr>
    </tbody>
</table>


<table>
    <thead>
        <tr>
            <th colspan="2">HSRP IP-címek</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td colspan="2"><u>Router17</u></td>
        </tr>
        <tr>
            <td><i>Interfész</i></td>
            <td><i>IP-cím</i></td>
        </tr>
        <tr>
            <td>GigabitEthernet8/0.10</td>
            <td>192.168.0.195</td>
        </tr>
        <tr>
            <td>GigabitEthernet8/0.20</td>
            <td>192.168.0.3</td>
        </tr>
        <tr>
            <td>GigabitEthernet8/0.30</td>
            <td>192.168.0.67</td>
        </tr>
        <tr>
            <td>GigabitEthernet8/0.50</td>
            <td>192.168.0.163</td>
        </tr>
        <tr>
            <td>GigabitEthernet8/0.99</td>
            <td>192.168.0.147</td>
        </tr>
        <tr>
            <td colspan="2"><u>Router1</u></td>
        </tr>
        <tr>
            <td><i>Interfész</i></td>
            <td><i>IP-cím</i></td>
        </tr>
        <tr>
            <td>GigabitEthernet7/0.10</td>
            <td>192.168.0.195</td>
        </tr>
        <tr>
            <td>GigabitEthernet7/0.20</td>
            <td>192.168.0.3</td>
        </tr>
        <tr>
            <td>GigabitEthernet7/0.30</td>
            <td>192.168.0.67</td>
        </tr>
        <tr>
            <td>GigabitEthernet7/0.50</td>
            <td>192.168.0.163</td>
        </tr>
        <tr>
            <td>GigabitEthernet7/0.99</td>
            <td>192.168.0.147</td>
        </tr>
    </tbody>
</table>


### Raktár

<table>
    <thead>
        <tr>
            <th colspan="2">Management</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>VLAN szám</td>
            <td>10</td>
        </tr>
        <tr>
            <td>Hálózati cím</td>
            <td>192.168.1.128</td>
        </tr>
        <tr>
            <td>Maszk (prefix);<br>
            összesen felhasználható címek</td>
            <td>255.255.255.240 (/28); 14 host</td>
        </tr>
        <tr>
            <td>Alapértelmezett átjáró</td>
            <td>192.168.1.130</td>
        </tr>
        <tr>
            <td>Beállított DNS-cím</td>
            <td></td>
        </tr>
        <tr>
            <td colspan="2"><i>Eszközök:</i></td>
        </tr>
    </tbody>
</table>


<table>
    <thead>
        <tr>
            <th colspan="2">Dolgozok</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>VLAN szám</td>
            <td>20</td>
        </tr>
        <tr>
            <td>Hálózati cím</td>
            <td>192.168.1.0</td>
        </tr>
        <tr>
            <td>Maszk (prefix);<br>
            összesen felhasználható címek</td>
            <td>255.255.255.128 (/25); 126 host</td>
        </tr>
        <tr>
            <td>Alapértelmezett átjáró</td>
            <td>192.168.1.2</td>
        </tr>
        <tr>
            <td>Beállított DNS-cím</td>
            <td></td>
        </tr>
        <tr>
            <td colspan="2"><i>Eszközök:</i></td>
        </tr>
    </tbody>
</table>



### Home Office

<table>
    <thead>
        <tr>
            <th colspan="2">Rendszergazdák</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>VLAN szám</td>
            <td>-</td>
        </tr>
        <tr>
            <td>Hálózati cím</td>
            <td>X</td>
        </tr>
        <tr>
            <td>Maszk (prefix);<br>
            összesen felhasználható címek</td>
            <td>X (/Y); Z host</td>
        </tr>
        <tr>
            <td>Alapértelmezett átjáró</td>
            <td></td>
        </tr>
        <tr>
            <td>Beállított DNS-cím</td>
            <td></td>
        </tr>
        <tr>
            <td colspan="2"><i>Eszközök:</i></td>
        </tr>
    </tbody>
</table>



### ISP

<table>
    <thead>
        <tr>
            <th colspan="2">Rendszergazdák</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>VLAN szám</td>
            <td>-</td>
        </tr>
        <tr>
            <td>Hálózati cím</td>
            <td>X</td>
        </tr>
        <tr>
            <td>Maszk (prefix);<br>
            összesen felhasználható címek</td>
            <td>X (/Y); Z host</td>
        </tr>
        <tr>
            <td>Alapértelmezett átjáró</td>
            <td></td>
        </tr>
        <tr>
            <td>Beállított DNS-cím</td>
            <td></td>
        </tr>
        <tr>
            <td colspan="2"><i>Eszközök:</i></td>
        </tr>
    </tbody>
</table>