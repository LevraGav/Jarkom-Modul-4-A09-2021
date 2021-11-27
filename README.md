# Jarkom-Modul-4-A09-2021
Laporan Resmi Praktikum Jarkom Modul 4

# Anggota Kelompok
Anggota  | NRP
---------|-------
Arvel Gavrilla Raissananda | 05111940000040
Johnivan Aldo Sudiono | 05111940000051
Vincent Yonathan | 05111940000186

## Soal Jarkom-Modul-2 2021
- [Soal](https://docs.google.com/document/d/1hf5Vi5nbEq6YY-nqmK7XUTHGNL_KVEFVc14mW9k0FAg/edit)

## Pendahuluan
![image](https://user-images.githubusercontent.com/36225278/143553295-d3dd4ebe-0225-4c75-92df-c02dc52663e5.png)

Dalam mengerjakan soal ini, kami menggunakan teknik VLSM (Variable Length Subnet Masking) menggunakan CPT (Cisco Packet Tracer), dan teknik CIDR (Classless Inter Domain Routing) menggunakan GNS 3

## VLSM (Variable Length Subnet Masking) - CPT

## CIDR (Classless Inter Domain Routing) - GNS3

Menggabungkan subnet-subnet paling bawah dalam topologi, berikut penggabungannya:

![image](https://user-images.githubusercontent.com/36225278/143669280-02c5d18a-351f-42a9-9454-b127423a9298.png)

![image](https://user-images.githubusercontent.com/36225278/143669286-e6432d2e-91e7-4eee-a844-fc93cdd131b3.png)

![image](https://user-images.githubusercontent.com/36225278/143669290-5c25f4b5-82bf-4356-998c-7f1a0b97140d.png)

![image](https://user-images.githubusercontent.com/36225278/143669298-31bf0094-039b-4dce-98e3-da4c83bf5280.png)

![image](https://user-images.githubusercontent.com/36225278/143669302-34603afe-0e79-4afc-b289-0924b985399e.png)

![image](https://user-images.githubusercontent.com/36225278/143669304-d769a7ee-3eea-4526-8509-bbd15d43ec6e.png)

![image](https://user-images.githubusercontent.com/36225278/143669312-04f69c52-76d6-4857-acaf-85f3ead428cc.png)

### Membuat topologi di GNS3

![image](https://user-images.githubusercontent.com/36225278/143669362-2b98c6a0-adf5-4859-940a-06c77a57013b.png)

### Membuat konfigurasi pada GNS3

#### Foosha
```
auto eth0
iface eth0 inet dhcp

auto eth1
iface eth1 inet static
        address 192.173.64.1
        netmask 255.255.255.252

auto eth2
iface eth2 inet static
         address 192.173.192.1
         netmask 255.255.255.252

auto eth3
iface eth3 inet static
        address 192.173.1.1
        netmask 255.255.255.252

auto eth4
iface eth4 inet static
        address 192.173.32.1
        netmask 255.255.255.252
```

#### Water 7
```
auto eth0
iface eth0 inet static
       address 192.173.192.2
       netmask 255.255.255.252
       gateway 192.173.192.1
auto eth1
iface eth1 inet static
       address 192.173.144.1
       netmask 255.255.255.252
auto eth2
iface eth2 inet static
         address 192.173.160.1
         netmask 255.255.252.0
```

#### Pucci
```
auto eth0
iface eth0 inet static
         address 192.173.144.2
         netmask 255.255.255.252
         gateway 192.186.144.1
auto eth1
iface eth1 inet static
         address 192.173.136.1
         netmask 255.255.255.128
auto eth2
iface eth2 inet static
         address 192.173.128.1
         netmask 255.255.248.0
```

#### Guanhao
```
auto eth0
iface eth0 inet static
          address 192.173.32.2
          netmask 255.255.255.252
          gateway 192.173.32.1
auto eth1
iface eth1 inet static
          address 192.173.20.1
          netmask 255.255.252.0
auto eth2
iface eth2 inet static
          address 192.173.8.1
          netmask 255.255.255.252
auto eth3
iface eth3 inet static
           address 192.173.16.1
          netmask 255.255.254.0
```

#### Alabasta
```
auto eth0
iface eth0 inet static
       address 192.173.18.1
       netmask 255.255.254.0
auto eth1
iface eth1 inet static
       address 192.173.16.2
       netmask 255.255.255.240
       gateway 192.173.16.1
```

#### Oimo
```
auto eth0
iface eth0 inet static
         address 192.173.8.2
         netmask 255.255.255.252
         gateway 192.173.8.1
auto eth1
iface eth1 inet static
          address 192.173.4.1
          netmask 255.255.255.0
auto eth2
iface eth2 inet static
           address 192.173.1.5
           netmask 255.255.255.252
```

#### Seastone
```
auto eth0
iface eth0 inet static
        address 192.173.4.2
        netmask 255.255.255.0
        gateway 192.186.4.1
auto eth1
iface eth1 inet static
        address 192.173.0.1
        netmask 255.255.252.0
```

#### Blueno
```
auto eth0
iface eth0 inet static
        address 192.173.64.2
        netmask 255.255.252.0
        gateway 192.173.64.1
```

#### Chiper
```
auto eth0
iface eth0 inet static
       address 192.173.160.2
       netmask 255.255.252.0
       gateway 192.173.160.1
```

#### Jipangu
```
auto eth0
iface eth0 inet static
	     address 192.173.136.2
	     netmask 255.255.255.128
	     gateway 192.173.136.1
```

#### Calmbert
```
auto eth0
iface eth0 inet static
	     address 192.173.128.2
	     netmask 255.255.248.0
	     gateway 192.173.128.1
```

#### Courtyard
```
auto eth0
iface eth0 inet static
       address 192.173.128.3
       netmask 255.255.248.0
       gateway 192.173.128.1
```

#### Jabra
```
auto eth0
iface eth0 inet static
        address 192.173.20.2
        netmask 255.255.252.0
        gateway 192.173.20.1
```

#### EnniesLobby
```
auto eth0
iface eth0 inet static
         address 192.173.4.3
         netmask 255.255.255.0
         gateway 192.173.4.1
```

#### Elena
```
auto eth0
iface eth0 inet static
         address 192.173.0.2
         netmask 255.255.252.0
         gateway 192.173.0.1
```

#### MainGate
```
auto eth0
iface eth0 inet static
      address 192.173.16.3
      netmask 255.255.254.0
      gateway 192.173.16.1
```

#### Jorge
```
auto eth0
iface eth0 inet static
         address 192.173.18.2
         netmask 255.255.255.240
         gateway 192.173.18.1
```
