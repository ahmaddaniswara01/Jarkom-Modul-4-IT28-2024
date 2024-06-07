# Jarkom-Modul-4-IT28-2024

## Anggota Kelompok IT28

| Nama  | NRP | 
| ----------- | ----------- |
| Angella Christie | 5027221047 | 
| Ahmad Fauzan Daniswara | 5027221057 |

# GNS 3 CIDR

## Topologi
![Screenshot 2024-06-08 002958](https://github.com/ahmaddaniswara01/Jarkom-Modul-4-IT28-2024/assets/131789727/e792bbc3-564b-497a-953e-829041f82d30)

## Tree
![jarkom modul 4](https://github.com/ahmaddaniswara01/Jarkom-Modul-4-IT28-2024/assets/131789727/75227d04-299b-4fe9-93e8-f8b13a12158a)

![tree-cidr](https://github.com/ahmaddaniswara01/Jarkom-Modul-4-IT28-2024/assets/131789727/dec8440d-1f71-45f0-91c0-6b76ff882708)

## Pembagian CIDR
![Screenshot 2024-06-08 003211](https://github.com/ahmaddaniswara01/Jarkom-Modul-4-IT28-2024/assets/131789727/676b3b90-f556-410f-b072-84595ca9a8b6)

![Screenshot 2024-06-08 003232](https://github.com/ahmaddaniswara01/Jarkom-Modul-4-IT28-2024/assets/131789727/91419e70-a25e-4612-9f3b-e25d70c84d9b)

![Screenshot 2024-06-08 003303](https://github.com/ahmaddaniswara01/Jarkom-Modul-4-IT28-2024/assets/131789727/38a42db2-1d02-4ea5-a887-4c421af16488)

## Pembagian IP
| Subnet | Network ID    | Netmask                | Broadcast      | Range IP                        |
|--------|---------------|------------------------|----------------|---------------------------------|
| A1     | 192.247.20.0  | 255.255.255.248 (/29)  | 192.247.20.7   | 192.247.20.1 - 192.247.20.6     |
| A2     | 192.247.17.0  | 255.255.255.192 (/26)  | 192.247.17.63  | 192.247.17.1 - 192.247.17.62    |
| A3     | 192.247.18.0  | 255.255.255.224 (/27)  | 192.247.18.31  | 192.247.18.1 - 192.247.18.30    |
| A4     | 192.247.21.0  | 255.255.255.252 (/30)  | 192.247.21.3   | 192.247.21.1 - 192.247.21.2     |
| A5     | 192.247.21.4  | 255.255.255.252 (/30)  | 192.247.21.7   | 192.247.21.5 - 192.247.21.6     |
| A6     | 192.247.14.0  | 255.255.255.0 (/24)    | 192.247.14.255 | 192.247.14.1 - 192.247.14.254   |
| A7     | 192.247.21.8  | 255.255.255.252 (/30)  | 192.247.21.11  | 192.247.21.9 - 192.247.21.10    |
| A8     | 192.247.19.0  | 255.255.255.240 (/28)  | 192.247.19.15  | 192.247.19.1 - 192.247.19.14    |
| A9     | 192.247.0.0   | 255.255.248.0 (/21)    | 192.247.7.255  | 192.247.0.1 - 192.247.7.254     |
| A10    | 192.247.8.0   | 255.255.252.0 (/22)    | 192.247.11.255 | 192.247.8.1 - 192.247.11.254    |
| A11    | 192.247.17.64 | 255.255.255.192 (/26)  | 192.247.17.127 | 192.247.17.65 - 192.247.17.126  |
| A12    | 192.247.21.12 | 255.255.255.252 (/30)  | 192.247.21.15  | 192.247.21.13 - 192.247.21.14   |
| A13    | 192.247.21.16 | 255.255.255.252 (/30)  | 192.247.21.19  | 192.247.21.17 - 192.247.21.18   |
| A14    | 192.247.12.0  | 255.255.254.0 (/23)    | 192.247.13.255 | 192.247.12.1 - 192.247.13.254   |
| A15    | 192.247.21.20 | 255.255.255.252 (/30)  | 192.247.21.23  | 192.247.21.21 - 192.247.21.22   |
| A16    | 192.247.21.24 | 255.255.255.252 (/30)  | 192.247.21.27  | 192.247.21.25 - 192.247.21.26   |
| A17    | 192.247.15.0  | 255.255.255.0 (/24)    | 192.247.15.255 | 192.247.15.1 - 192.247.15.200   |
| A18    | 192.247.19.16 | 255.255.255.240 (/28)  | 192.247.19.31  | 192.247.19.17 - 192.247.19.30   |
| A19    | 192.247.21.28 | 255.255.255.252 (/30)  | 192.247.21.31  | 192.247.21.29 - 192.247.21.30   |
| A20    | 192.247.16.0  | 255.255.255.128 (/25)  | 192.247.16.127 | 192.247.16.1 - 192.247.16.126   |
| A21    | 192.247.19.32 | 255.255.255.240 (/28)  | 192.247.19.47  | 192.247.19.33 - 192.247.19.46   |

## IP Configuration
### Jawa 
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet dhcp

auto eth1
iface eth1 inet static
address 192.247.20.1
netmask 255.255.255.252

auto eth2
iface eth2 inet static
address 192.247.21.1
netmask 255.255.255.252

auto eth3
iface eth3 inet static
address 192.247.21.21
netmask 255.255.255.252
```

### Sulawesi A1-A2-A11
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
address 192.247.20.2
netmask 255.255.255.252
gateway 192.247.0.1

auto eth1
iface eth1 inet static
address 192.247.17.1
netmask 255.255.255.192

auto eth2
iface eth2 inet static
address 192.247.17.65
netmask 255.255.255.192
```

### PC-Gorontalo A2
```
auto eth0
iface eth0 inet static
address 192.247.17.2
netmask 255.255.255.192
gateway 192.247.17.1
```

### PC-Marisa A2
```
auto eth0
iface eth0 inet static
address 192.247.17.3
netmask 255.255.255.192
gateway 192.247.17.1
```

### MALUKU-UTARA A2-A10
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
address 192.247.17.4
netmask 255.255.255.192
gateway 192.24717.1

auto eth1
iface eth1 inet static
address 192.247.8.1
netmask 255.255.255.224 
```

### PC-Ternate A10
```
auto eth0
iface eth0 inet static
address 192.247.8.2
netmask 255.255.252.192
gateway 192.247.8.1
```

### Server-PT Morotai A10
```
auto eth0
iface eth0 inet static
address 192.247.8.3
netmask 255.255.252.192
gateway 192.247.8.1
```

### PC-Tobelo A10
```
auto eth0
iface eth0 inet static
address 192.247.8.4
netmask 255.255.252.192
gateway 192.247.8.1
```

### BELAWA A11-A12
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
address 192.247.17.66
netmask 255.255.255.192
gateway 192.247.17.65

auto eth1
iface eth1 inet static
address 192.247.21.13
netmask 255.255.255.224
```

### PC-Madini A11
``` 
auto eth0
iface eth0 inet static
address 192.247.17.67
netmask 255.255.252.0
gateway 192.247.17.66
```

### PC-Baru A11
```
auto eth0
iface eth0 inet static
address 192.247.17.68
netmask 255.255.252.0
gateway 192.247.17.66
```

### MAKASAR A11-A12
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
address 192.247.17.69
netmask 255.255.255.192
gateway 192.247.17.65

auto eth1
iface eth1 inet static
address 192.247.21.14
netmask 255.255.255.224
```

### Server-PT Topejawa-Takalar A12
```
auto eth0
iface eth0 inet static
address 192.247.21.15
netmask 255.255.252.0
gateway 192.247.21.14
```

### Server-PT Galesong A12
```
auto eth0
iface eth0 inet static
address 192.247.21.16
netmask 255.255.252.0
gateway 192.247.21.14
```

### KALIMANTAN A4-A5
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
address 192.247.21.2
netmask 255.255.255.252
gateway 192.247.21.1

auto eth1
iface eth1 inet static
address 192.247.21.5
netmask 255.255.255.252
```

### KALIMANTAN-UTARA A5-A6-A13
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
address 192.247.21.6
netmask 255.255.255.252
gateway 192.247.21.5

auto eth1
iface eth1 inet static
address 192.247.14.1
netmask 255.255.252.0

auto eth2
iface eth2 inet static
address 192.247.21.17
netmask 255.255.255.252
```

### KALIMANTAN-TIMUR A13-A14-A7
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
address 192.247.21.18
netmask 255.255.255.252
gateway 192.247.21.17

auto eth1
iface eth1 inet static
address 192.247.12.1
netmask 255.255.254.0

auto eth2
iface eth2 inet static
address 192.247.21.9
netmask 255.255.255.252
```

### KALIMANTAN-SELATAN A13-A8-A9
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
address 192.247.21.19
netmask 255.255.255.252
gateway 192.247.21.18

auto eth1
iface eth1 inet static
address 192.247.19.1
netmask 255.255.252.240

auto eth2
iface eth2 inet static
address 192.247.0.1
netmask 255.255.248.0 
```

### PC-Selimau A6
```
auto eth0
iface eth0 inet static
address 192.247.14.2
netmask 255.255.255.0
gateway 192.247.14.1
```

### Server-PT Bangkirai A14
```
auto eth0
iface eth0 inet static
address 192.247.12.2
netmask 255.255.254.0
gateway 192.247.12.1
```

### PC-Lamaru A14
```
auto eth0
iface eth0 inet static
address 192.247.12.3
netmask 255.255.254.0
gateway 192.247.12.1
```

### PC-Angsana A8
```
auto eth0
iface eth0 inet static
address 192.247.19.2
netmask 255.255.255.2400
gateway 192.247.19.1
```

### PC-Bajuin A9
```
auto eth0
iface eth0 inet static
address 192.247.0.2
netmask 255.255.248.0
gateway 192.247.0.1
```

### PC-Takisung A9
```
auto eth0
iface eth0 inet static
address 192.247.0.3
netmask 255.255.248.0
gateway 192.247.0.1
```

### PC-Batakan A9
```
auto eth0
iface eth0 inet static
address 192.247.0.4
netmask 255.255.248.0
gateway 192.247.0.1
```

### Sumatera A15-A16-A18
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
address 192.247.21.22
netmask 255.255.255.252
gateway 192.247.21.21

auto eth1
iface eth1 inet static
address 192.247.21.25
netmask 255.255.255.252

auto eth2
iface eth2 inet static
address 192.247.19.17
netmask 255.255.255.240
```

### Lampung A16-A17
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
address 192.247.21.26
netmask 255.255.255.252
gateway 192.247.21.25

auto eth1
iface eth1 inet static
address 192.247.15.1
netmask 255.255.255.0
```

### PC-Sebuku A17
```
auto eth0
iface eth0 inet static
address 192.247.15.2
netmask 255.255.255.0
gateway 192.247.15.1
```

### Server-PT Sebesi A17
```
auto eth0
iface eth0 inet static
address 192.247.15.3
netmask 255.255.255.0
gateway 192.247.15.1
```

### Sumatera-Utara A18-A19
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
address 192.247.19.18
netmask 255.255.255.240
gateway 192.247.19.17

auto eth1
iface eth1 inet static
address 192.247.21.29
netmask 255.255.255.252
```

### PC-SAMOSIR A18
```
auto eth0
iface eth0 inet static
address 192.247.19.19
netmask 255.255.255.0
gateway 192.247.21.22
```

### PC-SIBANDANG A18
```
auto eth0
iface eth0 inet static
address 192.247.19.19
netmask 255.255.255.0
gateway 192.247.21.22
```

### Aceh A19-A20-A21
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet static
address 192.247.21.30
netmask 255.255.255.252
gateway 192.247.21.29

auto eth1
iface eth1 inet static
address 192.247.16.1
netmask 255.255.255.128

auto eth2
iface eth2 inet static
address 192.247.19.33
netmask 255.255.255.240
```

### PC-Berawang Tampu A20
```
auto eth0
iface eth0 inet static
address 192.247.16.2
netmask 255.255.255.0
gateway 192.247.16.1
```

### PC-Enang-Enang A20
```
auto eth0
iface eth0 inet static
address 192.247.16.3
netmask 255.255.255.0
gateway 192.247.16.1
```

### PC-Starland A20
```
auto eth0
iface eth0 inet static
address 192.247.16.4
netmask 255.255.255.0
gateway 192.247.16.1
```

### PC-Sabang A21
```
auto eth0
iface eth0 inet static
address 192.247.19.34
netmask 255.255.255.0
gateway 192.247.19.33
```

### PC-Lambaro A21
```
auto eth0
iface eth0 inet static
address 192.247.19.35
netmask 255.255.255.0
gateway 192.247.19.33
```

## ROUTING

### ACEH
```
# Ke Sumatera Utara
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.247.21.29
```

### LAMPUNG
```
#Ke Sumatera 
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.247.21.25
```

### KALIMANTAN SELATAN
```
#Ke Kalimantan TImur
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.247.21.8
```

### MAKASAR
```
#Ke Sulawesi
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.247.17.65
```

###BELAWA
```
#Ke Sulawesi
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.247.17.65
```

### MALUKU UTARA
```
#Ke Sulawesi
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.247.17.1
```

### SUMATERA UTARA
```
route add -net 192.247.16.0 netmask 255.255.255.128 gw 192.247.21.30 #SW-BLANGKARAI
route add -net 192.247.19.32 netmask 255.255.255.240 gw 192.247.21.30 #SW-BANDA-ACEH
```

### SUMATERA
```
#Ke Jawa 
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.247.21.21

#KE SUMATERA-UTARA
route add -net 192.247.21.28 netmask 255.255.255.252 gw 192.247.19.18
route add -net 192.247.16.0 netmask 255.255.255.128 gw 192.247.19.18
route add -net 192.247.19.32 netmask 255.255.255.240 gw 192.247.19.18

#KE LAMPUNG
route add -net 192.247.15.0 netmask 255.255.255.0 gw 192.247.21.26
```

KALIMANTAN TIMUR 
```
route add -net 192.247.19.0 netmask 255.255.255.240 gw 192.247.21.19
route add -net 192.247.0.0 netmask 255.255.248.0 gw 192.247.21.19
```

### KALIMANTAN UTARA
```
route add -net 192.247.12.0 netmask 255.255.254.0 gw 192.247.21.18
route add -net 192.247.21.8 netmask 255.255.255.252 gw 192.247.21.18
route add -net 192.247.19.0 netmask 255.255.255.240 gw 192.247.21.18
route add -net 192.247.0.0 netmask 255.255.248.0 gw 192.247.21.18
```

### KALIMANTAN
```
route add -net 192.247.21.16 netmask 255.255.255.252 gw 192.247.21.6
route add -net 192.247.12.0 netmask 255.255.254.0 gw 192.247.21.6
route add -net 192.247.21.8 netmask 255.255.255.252 gw 192.247.21.6
route add -net 192.247.19.0 netmask 255.255.255.240 gw 192.247.21.6
route add -net 192.247.0.0 netmask 255.255.248.0 gw 192.247.21.6
```

### SULAWESI
```
#KE MALUKU-UTARA
route add -net 192.247.8.0 netmask 255.255.252.0 gw 192.247.17.3

#KE MAKASAR
route add -net 192.247.21.12 netmask 255.255.255.252 gw 192.247.17.69

#KE BELAWA
route add -net 192.247.17.64 netmask 255.255.255.192 gw 192.247.17.66
```

### JAWA
```
#arah ke SUMATERA
route add -net 192.247.21.24 netmask 255.255.255.252 gw 192.247.21.22
route add -net 192.247.15.0 netmask 255.255.255.0 gw 192.247.21.22
route add -net 192.247.19.16 netmask 255.255.255.240 gw 192.247.21.22
route add -net 192.247.21.28 netmask 255.255.255.252 gw 192.247.21.22
route add -net 192.247.16.0 netmask 255.255.255.128 gw 192.247.21.22
route add -net 192.247.19.32 netmask 255.255.255.240 gw 192.247.21.22

#Ke arah KALIMANTAN
route add -net 192.247.21.4 netmask 255.255.255.252 gw 192.247.21.2
route add -net 192.247.14.0 netmask 255.255.255.0 gw 192.247.21.2
route add -net 192.247.21.16 netmask 255.255.255.252 gw 192.247.21.2
route add -net 192.247.12.0 netmask 255.255.254.0 gw 192.247.21.2
route add -net 192.247.21.8 netmask 255.255.255.252 gw 192.247.21.2
route add -net 192.247.19.0 netmask 255.255.255.240 gw 192.247.21.2
route add -net 192.247.0.0 netmask 255.255.248.0 gw 192.247.21.2

#Ke arah SULAWESI 
route add -net 192.247.17.64 netmask 255.255.255.192 gw 192.247.20.2
route add -net 192.247.21.12 netmask 255.255.255.252 gw 192.247.20.2
route add -net 192.247.18.0 netmask 255.255.255.224 gw 192.247.20.2
route add -net 192.247.17.0 netmask 255.255.255.192 gw 192.247.20.2
route add -net 192.247.8.0 netmask 255.255.252.0 gw 192.247.20.2
```

# Testing 
![Gambar WhatsApp 2024-06-06 pukul 23 00 38_e257e884](https://github.com/ahmaddaniswara01/Jarkom-Modul-4-IT28-2024/assets/131789727/091dcea8-1773-4d14-9727-2842b8546791)

![Gambar WhatsApp 2024-06-06 pukul 23 00 38_fb4bf5f1](https://github.com/ahmaddaniswara01/Jarkom-Modul-4-IT28-2024/assets/131789727/866722b8-949a-46e9-8d97-d9a0a3686807)

![Gambar WhatsApp 2024-06-06 pukul 23 00 37_5fa28fbf](https://github.com/ahmaddaniswara01/Jarkom-Modul-4-IT28-2024/assets/131789727/e7277d0b-b200-469b-a03a-ce06cb1851be)

![Gambar WhatsApp 2024-06-06 pukul 22 55 56_8aa80e8a](https://github.com/ahmaddaniswara01/Jarkom-Modul-4-IT28-2024/assets/131789727/6ace0ce5-23c1-4734-a705-1d857f216a05)

![Gambar WhatsApp 2024-06-06 pukul 22 55 56_1b7bba4a](https://github.com/ahmaddaniswara01/Jarkom-Modul-4-IT28-2024/assets/131789727/7f4d9b05-7b8c-4ea9-81f9-ae03e64d5248)

![Gambar WhatsApp 2024-06-06 pukul 22 55 54_6b012fcf](https://github.com/ahmaddaniswara01/Jarkom-Modul-4-IT28-2024/assets/131789727/5613bb2e-34a6-43a0-ab72-8f48f55893ab)

![Gambar WhatsApp 2024-06-06 pukul 22 55 54_3cff3f4e](https://github.com/ahmaddaniswara01/Jarkom-Modul-4-IT28-2024/assets/131789727/9d8d2cd2-ffa7-42a4-bcd0-f03754972517)
