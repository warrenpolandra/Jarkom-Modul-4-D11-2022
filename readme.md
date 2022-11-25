# Jarkom-Modul-4-D11-2022

## Kelompok D11:

- 5025201006 - Afira Rolobessy
- 5025201029 - Beryl
- 5025201233 - Warren Gerald Polandra

## Topologi

![Topologi](https://cdn.discordapp.com/attachments/856609726225973278/1044251635586707588/image.png)

## Cisco Packet Tracer - VLSM(Variable Length Subnet Masking)

### Pengelompokan Subnet

![Kelompok Subnet](https://cdn.discordapp.com/attachments/856609726225973278/1044298202754580540/image.png)

### Penghitungan Jumlah Subnet

| No | Subnet | Jumlah IP | Netmask |
| :---: | :---: | :---: | :---: |
| 1 |	A1 | 1001 | /22 |
| 2 | A8 | 501 | /23 |
| 3 | A16 | 271 | /23 |
| 4 | A5 | 251 | /24 |
| 5 | A6 | 212 | /24 |
| 6 | A11 | 121 | /25 |
| 7 | A17 | 121 | /25 |
| 8	| A18 | 71 | /25 |
| 9	| A2 | 51 | /26 |
| 10 | A3 | 2 | /30 |
| 11 | A4 | 2 | /30 |
| 12 | A7 | 2 | /30 |
| 13 | A10 | 2 | /30 |
| 14 | A9 | 2 | /30 |
| 15 | A12 | 2 | /30 |
| 16 | A13 | 2 | /30 |
| 17 | A14 | 2 | /30 |
| 18 | A15 | 2 | /30 |
| **Total** | **18** | **2168** | **/20** |

### VLSM Tree

![VLSM Tree](https://cdn.discordapp.com/attachments/856609726225973278/1044336173897744454/VLSM_Tree.drawio.png)

### Routing

#### Subnet A12

**The Resonance** menuju **The Order**

```
IP Address 192.190.0.21
Subnet Mask 255.255.255.252
```

**The Order** menuju **The Resonance**

```
IP Address 192.190.0.22
Subnet Mask 255.255.255.252
```

Static Route pada **The Order**

```
Network 0.0.0.0
Mask 0.0.0.0
Next hop 192.190.0.21
```

#### Subnet A2

**The Order** menuju **Ashaf**

```
IP Address 192.190.0.65
Subnet Mask 255.255.255.192
```

**Ashaf** menuju **The Order**

```
IP Address 192.190.0.66
Subnet Mask 255.255.255.192
Gateway 192.190.0.65
```

Static Route pada **The Resonance**

```
Network 192.190.0.64
Mask 255.255.255.192
Next hop 192.190.0.22
```

#### Subnet A3

**The Order** menuju **The Minister**

```
IP Address 192.190.0.1
Subnet Mask 255.255.255.252
```

**The Minister** menuju **The Order**

```
IP Address 192.190.0.2
Subnet Mask 255.255.255.252
```

Static Route pada **The Minister**

```
Network 0.0.0.0
Mask 0.0.0.0
Next hop 192.190.0.1
```

Static Route pada **The Resonance**

```
Network 192.190.0.0
Mask 255.255.255.252
Next hop 192.190.0.22
```

#### Subnet A1

**The Minister** menuju **Guideau**

```
IP Address 192.190.12.1
Subnet Mask 255.255.252.0
```

**Guideau** menuju **The Minister**

```
IP Address 192.190.12.2
Subnet Mask 255.255.252.0
Gateway 192.190.12.1
```

Static Route pada **The Order**

```
Network 192.190.12.0
Mask 255.255.252.0
Next hop 192.190.0.2
```

Static Route pada **The Resonance**

```
Network 192.190.12.0
Mask 255.255.252.0
Next hop 192.190.0.22
```

#### Subnet A4

**The Minister** menuju **The Dauntless**

```
IP Address 192.190.0.5
Subnet Mask 255.255.255.252
```

**The Dauntless** menuju **The Minister**

```
IP Address 192.190.0.6
Subnet Mask 255.255.255.252
```

Static Route pada **The Dauntless**

```
Network 0.0.0.0
Mask 0.0.0.0
Next hop 192.190.0.5
```

Static Route pada **The Order**

```
Network 192.190.0.4
Mask 255.255.255.252
Next hop 192.190.0.2
```

Static Route pada **The Resonance**

```
Network 192.190.0.4
Mask 255.255.255.252
Next hop 192.190.0.22
```

#### Subnet A5

**The Dauntless** menuju **Johan** dan **Phanora**

```
IP Address 192.190.1.1
Subnet Mask 255.255.255.0
```

**Johan** menuju **The Dauntless**

```
IP Address 192.190.1.2
Subnet Mask 255.255.255.0
Gateway 192.190.1.1
```

**Phanora** menuju **The Dauntless**

```
IP Address 192.190.1.3
Subnet Mask 255.255.255.0
Gateway 192.190.1.1
```

Static Route pada **The Minister**

```
Network 192.190.1.0
Mask 255.255.255.0
Next hop 192.190.0.6
```

Static Route pada **The Order**

```
Network 192.190.1.0
Mask 255.255.255.0
Next hop 192.190.0.2
```

Static Route pada **The Resonance**

```
Network 192.190.1.0
Mask 255.255.255.0
Next hop 192.190.0.22
```

#### Subnet A10

**The Resonance** menuju **The Instrument**

```
IP Address 192.190.0.17
Subnet Mask 255.255.255.252
```

**The Instrument** menuju **The Resonance**

```
IP Address 192.190.0.18
Subnet Mask 255.255.255.252
```

Static Route pada **The Instrument**

```
Network 0.0.0.0
Mask 0.0.0.0
Next hop 192.190.0.17
```

#### Subnet A11

**The Instrument** menuju **Matt Cugat**

```
IP Address 192.190.0.129
Subnet Mask 255.255.255.128
```

**Matt Cugat** menuju **The Instrument**

```
IP Address 192.190.0.130
Subnet Mask 255.255.255.128
Gateway 192.190.0.129
```

Static Route pada **The Resonance**

```
Network 192.190.0.128
Mask 255.255.255.128
Next hop 192.190.0.18
```

#### Subnet A9

**The Instrument** menuju **The Firefist**

```
IP Address 192.190.0.13
Subnet Mask 255.255.255.252
```

**The Firefist** menuju **The Instrument**

```
IP Address 192.190.0.14
Subnet Mask 255.255.255.252
```

Static Route pada **The Firefist**

```
Network 0.0.0.0
Mask 0.0.0.0
Next hop 192.190.0.13
```

Static Route pada **The Resonance**

```
Network 192.190.0.12
Mask 255.255.255.252
Next hop 192.190.0.18
```

#### Subnet A6

**The Firefist** menuju **Keith** dan **The Queen**

```
IP Address 192.190.9.1
Subnet Mask 255.255.255.0
```

**Keith** menuju **The Firefist**

```
IP Address 192.190.9.2
Subnet Mask 255.255.255.0
Gateway 192.190.9.1
```

**The Queen** menuju **The Firefist**

```
IP Address 192.190.9.3
Subnet Mask 255.255.255.0
```

Static Route pada **The Queen**

```
Network 0.0.0.0
Mask 0.0.0.0
Next hop 192.190.9.1
```

Static Route pada **The Instrument**

```
Network 192.190.9.0
Mask 255.255.255.0
Next hop 192.190.0.14
```

Static Route pada **The Resonance**

```
Network 192.190.9.0
Mask 255.255.255.0
Next hop 192.190.0.18
```

#### Subnet A7

**The Queen** menuju **The Witch**

```
IP Address 192.190.0.9
Subnet Mask 255.255.255.252
```

**The Witch** menuju **The Queen**

```
IP Address 192.190.0.10
Subnet Mask 255.255.255.252
Gateway 192.190.0.9
```

Static Route pada **The Firefist**

```
Network 192.190.0.8
Mask 255.255.255.252
Next hop 192.190.9.3
```

Static Route pada **The Instrument**

```
Network 192.190.0.8
Mask 255.255.255.252
Next hop 192.190.0.14
```

Static Route pada **The Resonance**

```
Network 192.190.0.8
Mask 255.255.255.252
Next hop 192.190.0.18
```

#### Subnet A8

**The Firefist** menuju **Oakleave**

```
IP Address 192.190.2.1
Subnet Mask 255.255.254.0
```

**Oakleave** menuju **The Firefist**

```
IP Address 192.190.2.2
Subnet Mask 255.255.254.0
Gateway 192.190.2.1
```

Static Route pada **The Instrument**

```
Network 192.190.2.0
Mask 255.255.254.0
Next hop 192.190.0.14
```

Static Route pada **The Resonance**

```
Network 192.190.2.0
Mask 255.255.254.0
Next hop 192.190.0.18
```

#### Subnet A15

**The Instrument** menuju **The Profound**

```
IP Address 192.190.0.57
Subnet Mask 255.255.255.252
```

**The Profound** menuju **The Instrument**

```
IP Address 192.190.0.58
Subnet Mask 255.255.255.252
```

Static Route pada **The Profound**

```
Network 0.0.0.0
Mask 0.0.0.0
Next hop 192.190.0.57
```

Static Route pada **The Resonance**

```
Netwprk 192.190.0.56
Mask 255.255.255.252
Next hop 192.190.0.18
```

#### Subnet A18

**The Profound** menuju **Helga**

```
IP Address 192.190.8.129
Subnet Mask 255.255.255.128
```

**Helga** menuju **The Profound**

```
IP Address 192.190.8.130
Subnet Mask 255.255.255.128
Gateway 192.190.8.129
```

Static Route pada **The Instrument**

```
Network 192.190.8.128
Mask 255.255.255.128
Next hop 192.190.0.58
```

Static Route pada **The Resonance**

```
Network 192.190.8.128
Mask 255.255.255.128
Next hop 192.190.0.18
```

#### Subnet A17

**The Profound** menuju **Spendrow**

```
IP Address 192.190.8.1
Subnet Mask 255.255.255.128
```

**Spendrow** menuju **The Profound**

```
IP Address 192.190.8.2
Subnet Mask 255.255.255.128
Gateway 192.190.8.1
```

Static Route pada **The Instrument**

```
Network 192.190.8.0
Mask 255.255.255.128
Next hop 192.190.0.58
```

Static Route pada **The Resonance**

```
Network 192.190.8.0
Mask 255.255.255.128
Next hop 192.190.0.18
```

#### Subnet A14

**The Resonance** menuju **The Magical**

```
IP Address 192.190.0.29
Subnet Mask 255.255.255.252
```

**The Magical** menuju **The Resonance**

```
IP Address 192.190.0.30
Subnet Mask 255.255.255.252
```

Static Route pada **The Magical**

```
Network 0.0.0.0
Mask 255.255.255.252
Next hop 192.190.0.29
```

#### Subnet A16

**The Magical** menuju **Coverkt** dan **Haines**

```
IP Address 192.190.10.1
Subnet Mask 255.255.254.0
```

**Coverkt** menuju **The Magical**

```
IP Address 192.190.10.2
Subnet Mask 255.255.254.0
Gateway 192.190.10.1
```

**Haines** menuju **The Magical**

```
IP Address 192.190.10.3
Subnet Mask 255.255.254.0
Gateway 192.190.10.1
```

Static Route pada **The Resonance**

```
Network 192.190.10.0
Mask 255.255.254.0
Next hop 192.190.0.30
```

#### Subnet A13

**The Resonance** menuju **The Beast**

```
IP Address 192.190.0.25
Subnet Mask 255.255.255.252
```

**The Beast** menuju **The Resonance**

```
IP Address 192.190.0.26
Subnet Mask 255.255.255.252
Gateway 192.190.0.25
```

## Graphical Network Simulator 3 - Classless Inter-Domain Routing

### Pengelompokan Subnet

#### Langkah 1 - Subnet level A

![CIDR A](https://cdn.discordapp.com/attachments/856609726225973278/1045766179714768957/Subnet_CIDR_A.png)

Subnet yang Digabungkan

| Subnet Baru | Anggota 1 | Anggota 2 | Netmask |
| :---: | :---: | :---: | :---: |
| A1 | Guideau | The Minister | /22 |
| A2 | The Minister | The Dauntless | /26 |
| A3 | The Minister | The Order | /30 |
| A4 | The Minister | The Dauntless | /30 |
| A5 | The Dauntless | Phanora, Johan | /24 |
| A6 | Keith | The Firefist, The Queen | /24 |
| A7 | The Witch | The Queen | /30 |
| A8 | Oakleave | The Firefist | /23 |
| A9 | The Instrument | The Firefist | /30 |
| A10 | The Resonance | The Instrument | /30 |
| A11 | The Instrument | Matt Cugat | /25 |
| A12 | The Resonance | The Order | /30 |
| A13 | The Resonance | The Beast | /30 |
| A14 | The Resonance | The Magical | /30 |
| A15 | The Instrument | The Profound | /30 |
| A16 | The Magical | Corvekt, Haines | /23 |
| A17 | The Profound | Spendrow | /25 |
| A18 | The Profound | Helga | /25 |

#### Langkah 2 - Subnet level B

![CIDR B](https://cdn.discordapp.com/attachments/856609726225973278/1045766180159356928/Subnet_CIDR_B.png)

| Subnet Baru | Anggota 1 | Anggota 2 | Netmask |
| :---: | :---: | :---: | :---: |
| B1 | A5 (/24) | A4 (/30) | /23 |
| B2 | A7 (/30) | A6 (/24) | /23 |
| B3 | A14 (/30) | A16 (/23) | /22 |
| B4 | A18 (/25) | A17 (/25) | /24 |

#### Langkah 3 - Subnet level C

![CIDR C](https://cdn.discordapp.com/attachments/856609726225973278/1045766176464175224/Subnet_CIDR_C.png)

| Subnet Baru | Anggota 1 | Anggota 2 | Netmask |
| :---: | :---: | :---: | :---: |
| C1 | B1 (/23) | A1 (/22) | /21 |
| C2 | B2 (/23) | A8 (/23) | /22 |
| C3 | B3 (/22) | A13 (/30) | /21 |
| C4 | B4 (/24) | A15 (/30) | /23 |

#### Langkah 4 - Subnet level D

![CIDR D](https://cdn.discordapp.com/attachments/856609726225973278/1045766176967499847/Subnet_CIDR_D.png)

| Subnet Baru | Anggota 1 | Anggota 2 | Netmask |
| :---: | :---: | :---: | :---: |
| D1 | C1 (/21) | A3 (/30) | /20 |
| D2 | C2 (/22) | A9 (/30) | /21 |
| D3 | C4 (/23) | A11 (/25) | /22 |

#### Langkah 5 - Subnet level E

![CIDR E](https://cdn.discordapp.com/attachments/856609726225973278/1045766177344978954/Subnet_CIDR_E.png)

| Subnet Baru | Anggota 1 | Anggota 2 | Netmask |
| :---: | :---: | :---: | :---: |
| E1 | D1 (/20) | A2 (/26) | /19 |
| E2 | D2 (/21) | D3 (/22) | /20 |

#### Langkah 6 - Subnet level F

![CIDR F](https://cdn.discordapp.com/attachments/856609726225973278/1045774056911294536/Subnet_CIDR_F.png)

| Subnet Baru | Anggota 1 | Anggota 2 | Netmask |
| :---: | :---: | :---: | :---: |
| F1 | E1 (/19) | A12 (/30) | /18 |
| F2 | E2 (/20) | A10 (/30) | /19 |

#### Langkah 7 - Subnet level G

![CIDR G](https://cdn.discordapp.com/attachments/856609726225973278/1045774057217466408/Subnet_CIDR_G.png)

| Subnet Baru | Anggota 1 | Anggota 2 | Netmask |
| :---: | :---: | :---: | :---: |
| G1 | F2 (/19) | C3 (/21) | /18 |

#### Langkah 8 - Subnet level H

![CIDR H](https://cdn.discordapp.com/attachments/856609726225973278/1045774056466694324/Subnet_CIDR_H.png)

| Subnet Baru | Anggota 1 | Anggota 2 | Netmask |
| :---: | :---: | :---: | :---: |
| H1 | F1 (/18) | G1 (/18) | /17 |

### CIDR Tree

![CIDR Tree](https://cdn.discordapp.com/attachments/856609726225973278/1045775454575001710/CIDR_Tree.png)

### Network Configuration

Setelah mendapatkan pembagian IP, dilakukan network configuration untuk setiap node yang ada

#### The Resonance

```
auto eth0
iface eth0 inet dhcp

auto eth1
iface eth1 inet static
    address 192.190.32.1
    netmask 255.255.255.252

auto eth2
iface eth2 inet static
    address 192.190.80.1
    netmask 255.255.255.252

auto eth3
iface eth3 inet static
    address 192.190.98.1
    netmask 255.255.255.252

auto eth4
iface eth4 inet static
    address 192.190.100.1
    netmask 255.255.255.252
```

#### The Order

```
auto eth0
iface eth0 inet static
    address 192.190.32.2
    netmask 255.255.255.252
    gateway 192.190.32.1

auto eth1
iface eth1 inet static
    address 192.190.16.1
    netmask 255.255.255.192

auto eth2
iface eth2 inet static
    address 192.190.8.1
    netmask 255.255.255.252
```

#### Ashaf (50 host)

```
auto eth0
iface eth0 inet static
    address 192.190.16.2
    netmask 255.255.255.192
    gateway 192.190.16.1
```

#### The Minister

```
auto eth0
iface eth0 inet static
    address 192.190.8.2
    netmask 255.255.255.252
    gateway 192.190.8.1

auto eth1
iface eth1 inet static
    address 192.190.4.1
    netmask 255.255.252.0

auto eth2
iface eth2 inet static
    address 192.190.1.1
    netmask 255.255.255.252
```

#### Guideau (1000 host)

```
auto eth0
iface eth0 inet static
    address 192.190.4.2
    netmask 255.255.255.0
    gateway 192.190.4.1
```

#### The Dauntless

```
auto eth0
iface eth0 inet static
    address 192.190.1.2
    netmask 255.255.255.252
    gateway  192.190.1.1

auto eth1
iface eth1 inet static
    address 192.190.0.1
    netmask 255.255.255.0
```

#### Johan (100 host)

```
auto eth0
iface eth0 inet static
    address 192.190.0.2
    netmask 255.255.255.0
    gateway 192.190.0.1
```

#### Phanora (150 host)

```
auto eth0
iface eth0 inet static
    address 192.190.0.3
    netmask 255.255.255.0
    gateway 192.190.0.1
```

#### The Instrument

```
auto eth0
iface eth0 inet static
    address 192.190.80.2
    netmask 255.255.255.252
    gateway 192.190.80.1

auto eth1
iface eth1 inet static
    address 192.190.74.1
    netmask 255.255.255.128

auto eth2
iface eth2 inet static
    address 192.190.68.1
    netmask 255.255.255.252

auto eth3
iface eth3 inet static
    address 192.190.73.1
    netmask 255.255.255.252
```

#### Matt Cugat (120 host)

```
auto eth0
iface eth0 inet static
    address 192.190.74.2
    netmask 255.255.255.128
    gateway 192.190.74.1
```

#### The Firefist

```
auto eth0
iface eth0 inet static
    address 192.190.68.2
    netmask 255.255.255.252
    gateway 192.190.68.1

auto eth1
iface eth1 inet static
    address 192.190.64.1
    netmask 255.255.255.0

auto eth2
iface eth2 inet static
    address 192.190.66.1
    netmask 255.255.254.0
```

#### Keith (210 host)

```
auto eth0
iface eth0 inet static
    address 192.190.64.2
    netmask 255.255.255.0
    gateway 192.190.64.1
```

#### The Queen

```
auto eth0
iface eth0 inet static
    address 192.190.64.3
    netmask 255.255.255.0
    gateway 192.190.64.1

auto eth1
iface eth1 inet static
    address 192.190.65.1
    netmask 255.255.255.252
```

#### The Witch

```
auto eth0
iface eth0 inet static
    address 192.190.65.2
    netmask 255.255.255.252
    gateway 192.190.65.1
```

#### Oakleave (500 host)

```
auto eth0
iface eth0 inet static
    address 192.190.66.2
    netmask 255.255.254.0
    gateway 192.190.66.1
```

#### The Profound

```
auto eth0
iface eth0 inet static
    address 192.190.73.2
    netmask 255.255.255.252
    gateway 192.190.73.1

auto eth1
iface eth1 inet static
    address 192.190.72.129
    netmask 255.255.255.128

auto eth2
iface eth2 inet static
    address 192.190.72.1
    netmask 255.255.255.128
```

#### Helga (70 host)

```
auto eth0
iface eth0 inet static
    address 192.190.72.130
    netmask 255.255.255.128
    gateway 192.190.72.129
```

#### Spendrow (120 host)

```
auto eth0
iface eth0 inet static
    address 192.190.72.2
    netmask 255.255.255.128
    gateway 192.190.72.1
```

#### The Magical

```
auto eth0
iface eth0 inet static
    address 192.190.98.2
    netmask 255.255.255.252
    gateway 192.190.98.1

auto eth1
iface eth1 inet static
    address 192.190.96.1
    netmask 255.255.254.0
```

#### Coverkt (200 host)

```
auto eth0
iface eth0 inet static
    address 192.190.96.2
    netmask 255.255.254.0
    gateway 192.190.96.1
```

#### Haines (70 host)

```
auto eth0
iface eth0 inet static
    address 192.190.96.3
    netmask 255.255.254.0
    gateway 192.190.96.1
```

#### The Beast

```
auto eth0
iface eth0 inet static
    address 192.190.100.2
    netmask 255.255.255.252
    gateway 192.190.100.1
```

### Routing

Setelah network configuration, dilakukan routing pada setiap router dan memasukkan nameserver pada setiap host dan router

#### Untuk Semua Host dan Server

```
echo nameserver 192.168.122.1 > /etc/resolv.conf
iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE -s 192.190.0.0/16
```

#### The Resonance

```
route add -net 192.190.16.0 netmask 255.255.255.192 gw 192.190.32.2
route add -net 192.190.8.0 netmask 255.255.255.252 gw 192.190.32.2
route add -net 192.190.4.0 netmask 255.255.252.0 gw 192.190.32.2
route add -net 192.190.1.0 netmask 255.255.255.252 gw 192.190.32.2
route add -net 192.190.0.0 netmask 255.255.255.0 gw 192.190.32.2

route add -net 192.190.74.0 netmask 255.255.255.128 gw 192.190.80.2
route add -net 192.190.68.0 netmask 255.255.255.252 gw 192.190.80.2
route add -net 192.190.64.0 netmask 255.255.255.0 gw 192.190.80.2
route add -net 192.190.65.0 netmask 255.255.255.252 gw 192.190.80.2
route add -net 192.190.66.0 netmask 255.255.254.0 gw 192.190.80.2
route add -net 192.190.73.0 netmask 255.255.255.252 gw 192.190.80.2
route add -net 192.190.72.128 netmask 255.255.255.128 gw 192.190.80.2
route add -net 192.190.72.0 netmask 255.255.255.128 gw 192.190.80.2

route add -net 192.190.96.0 netmask 255.255.254.0 gw 192.190.98.2
iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE -s 192.190.0.0/16
```

#### The Order

```
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.190.32.1
route add -net 192.190.4.0 netmask 255.255.252.0 gw 192.190.8.2
route add -net 192.190.0.0 netmask 255.255.255.0 gw 192.190.8.2
route add -net 192.190.1.0 netmask 255.255.255.252 gw 192.190.8.2

echo nameserver 192.168.122.1 > /etc/resolv.conf
iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE -s 192.190.0.0/16
```

#### The Minister

```
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.190.8.1
route add -net 192.190.0.0 netmask 255.255.255.0 gw 192.190.1.2

echo nameserver 192.168.122.1 > /etc/resolv.conf
iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE -s 192.190.0.0/16
```

#### The Dauntless

```
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.190.1.1

echo nameserver 192.168.122.1 > /etc/resolv.conf
iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE -s 192.190.0.0/16
```

#### The Instrument

```
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.190.80.1

route add -net 192.190.64.0 netmask 255.255.255.0 gw 192.190.68.2
route add -net 192.190.65.0 netmask 255.255.255.252 gw 192.190.68.2
route add -net 192.190.66.0 netmask 255.255.254.0 gw 192.190.68.2

route add -net 192.190.72.128 netmask 255.255.255.128 gw 192.190.73.2
route add -net 192.190.72.0 netmask 255.255.255.128 gw 192.190.73.2

echo nameserver 192.168.122.1 > /etc/resolv.conf
iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE -s 192.190.0.0/16
```

#### The Firefist

```
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.190.68.1
route add -net 192.190.65.0 netmask 255.255.255.252 gw 192.190.64.3

echo nameserver 192.168.122.1 > /etc/resolv.conf
iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE -s 192.190.0.0/16
```

#### The Queen

```
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.190.64.1

echo nameserver 192.168.122.1 > /etc/resolv.conf
iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE -s 192.190.0.0/16
```

#### The Profound

```
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.190.73.1

echo nameserver 192.168.122.1 > /etc/resolv.conf
iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE -s 192.190.0.0/16
```

#### The Magical

```
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.190.98.1

echo nameserver 192.168.122.1 > /etc/resolv.conf
iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE -s 192.190.0.0/16
```
