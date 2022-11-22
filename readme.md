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
| 9	| A2 | 51 | /23 |
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
