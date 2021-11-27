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
![Subnet](https://user-images.githubusercontent.com/72689610/143666832-4e7ec7c7-4413-4e79-9014-3594842bd332.png)

### 1. Jumlah Alamat IP
Subnet serta jumlah IP untuk mendapatkan netmask dari tiap subnet ditunjukkan oleh tabel berikut :
| Subnet  | Jumlah IP | Netmask |
| :---         |     :---:      |          ---: |
| ------------- | ------------- | ------------- |
| A1  | 721 | /22 |
| A2  | 252 | /24 |
| A3  | 13 | /28 |
| A4  | 502 | /23 |
| A5  | 521 | /22 |
| A6  | 2 | /30 |
| A7  | 2 | /30 |
| A8  | 2 | /30 |
| A9  | 701 | /22 |
| A10  | 2 | /30 |
| A11 | 2021 | /21 |
| A12  | 101 | /25 |
| A13  | 1001 | /22 |
| Total  | 5841 | /19 |

### 2. Menghitung NID dengan tree (pohon)
Subnet pertama memiliki NID 192.173.0.0 dengan netmask /19. Perhitungan dengan pohon dapat dilihat sebagai berikut :
![image](https://user-images.githubusercontent.com/72689610/143667143-2b90879b-1ea2-41b6-a309-44405b72e3b7.png)

### [Link Tree](https://intip.in/PohonPembagianIpVSLM)

### 3. Pengaturan Konfigurasi IP
###	Foosha
1.	Cloud                                                        
    192.173.72.13 subnet 255.255.255.252
2.	Mengarah Blueno                                             
    192.173.16.1 subnet 255.255.252.0
3.	Mengarah Server Doriki                                                              
    192.173.0.33 subnet 255.255.255.240
4.	Mengarah Guanhao                                                                          
    192.173.0.5 subnet 255.255.255.252
5.	Mengarah Water7                                                                                           
    192.173.0.9 subnet 255.255.255.252                                        
                                                                                      
### Water7
1.	Mengarah Foosha                                                                     
    192.173.0.10 subnet 255.255.255.252
2.	Mengarah Cipher                                                                         
    192.173.12.1 subnet 255.255.255.0
3.	Mengarah Pucci                                                                                          
    192.173.0.13 subnet 255.255.255.252

###	Pucci
1.	Mengarah Water7                                                                                     
    192.173.0.14 subnet 255.255.255.252
2.	Mengarah Jipangu                                                                                
    192.173.0.129 subnet 255.255.255.128
3.	Mengarah Courtyard dan Calmbelt                                                                             
    192.173.24.1 subnet 255.255.248.0

###	Guanhao
1.	Mengarah Foosha                                                                     
    192.173.0.6 subnet 255.255.255.252
2.	Mengarah Jabra                                                                                      
    192.173.8.1 subnet 255.255.252.0
3.	Mengarah Alabasta                                                                     
    192.173.2.1 subnet 255.255.254.0
4.	Mengarah OIMO                                                                   
    192.173.0.1 subnet 255.255.255.252

###	Alabasta 
1.	Mengarah Guanhao                                                                                                                                                          
    192.173.2.2 subnet 255.255.254.0 
2.	Mengarah Jorge                                                                                                   
    192.173.0.17 subnet 255.255.255.240

###	OIMO
1.	Mengarah Guanhao                                                          
    192.173.0.2 subnet 255.255.255.252
2.	Mengarah Server Fukurou                                                     
    192.173.0.49 subnet 255.255.255.240
3.	Mengarah Seastone                                                                 
    192.173.1.1 subnet 255.255.255.0
                          
###	Seastone
1.	Mengarah OIMO                                                                       
    192.173.1.2 subnet 255.255.255.0
2.	Mengarah Elena                                                                          
    192.173.4.1 subnet 255.255.252.0

###	PC Jipangu <br>
![image](https://user-images.githubusercontent.com/72689610/143667457-19da630b-b00e-42e7-ae2e-7835cd829f1f.png)

###	PC Courtyard <br>
![image](https://user-images.githubusercontent.com/72689610/143667641-ce5ef71e-8342-4c22-a88d-0113fa846109.png)

###	PC Calmbelt <br>
![image](https://user-images.githubusercontent.com/72689610/143667694-e975033e-cf3a-4eed-9aa8-221b214651d5.png) 

###	PC Cipher <br>
![image](https://user-images.githubusercontent.com/72689610/143667736-83d917d4-01f2-433c-9d44-7ca210a14a4b.png) 

###	PC Blueno <br>
![image](https://user-images.githubusercontent.com/72689610/143667790-0b616249-1898-42be-9c9d-c9e88eb8276c.png) 

###	PC Jabra <br>
![image](https://user-images.githubusercontent.com/72689610/143668090-7067edc6-c90a-4dea-84f6-56a5b584bea0.png) 

###	PC Maingate <br>
![image](https://user-images.githubusercontent.com/72689610/143668152-956ca995-5164-4504-9225-13b531d9c34c.png) 

###	PC Jorge <br>
![image](https://user-images.githubusercontent.com/72689610/143668172-3545fd5c-3f0a-4ac5-99d9-f51e67adee41.png) 

###	PC Enieslobby <br>
![image](https://user-images.githubusercontent.com/72689610/143668183-d978eeee-c20c-4728-b58b-c258c1c51865.png)

###	PC Elena <br>
![image](https://user-images.githubusercontent.com/72689610/143668285-c1f1db6d-0661-4cf6-a4a7-56fc87c204d3.png) 

###	Server Fukurou <br>
![image](https://user-images.githubusercontent.com/72689610/143668317-48c6abdb-b90a-4c00-a46f-33291399c47c.png) 

###	Server Doriki <br>
![image](https://user-images.githubusercontent.com/72689610/143668337-50820ab7-5d54-409a-8d8a-ce3ee0e409da.png)

### Pengaturan Routing
Untuk langkah nya bisa masuk kedalam router, lalu menekan menu static dan menambahkan data yang diinginkan

###	Foosha
- 192.173.4.0/22 via 192.173.0.6
- 192.173.1.0/24 via 192.173.0.6
- 192.173.0.16/28 via 192.173.0.6
- 192.173.2.0/23 via 192.173.0.6
- 192.173.8.0/22 via 192.173.0.6
- 192.173.0.0/30 via 192.173.0.6
- 192.173.12.0/22 via 192.173.0.10
- 192.173.0.12/30 via 192.173.0.10
- 192.173.0.128/25 via 192.173.0.10
- 192.173.0.48/28 via 192.173.0.6
- 192.173.24.0/21 via 192.173.0.10 

![image](https://user-images.githubusercontent.com/72689610/143668562-2edb69f4-f352-4c40-979a-4e2abe672e51.png)

###	Water7
- 0.0.0.0/0 via 192.173.0.9
- 192.173.24.0/21 via 192.173.0.14
- 192.173.0.128/25 via 192.173.0.14

![image](https://user-images.githubusercontent.com/72689610/143668799-80debd20-4f8f-4552-bb75-39675cd2af38.png)

###	Pucci
- 0.0.0.0/0 via 192.173.0.13

![image](https://user-images.githubusercontent.com/72689610/143669293-8fea625d-9d2d-4a9c-a665-db3a49184228.png)

### Guanhao
- 0.0.0.0/0 via 192.173.0.5
- 192.173.4.0/22 via 192.173.0.2
- 192.173.1.0/24 via 192.173.0.2
- 192.173.0.16/28 via 192.173.2.2
- 192.173.0.48/28 via 192.173.0.2

![image](https://user-images.githubusercontent.com/72689610/143669344-4b46cad0-c35d-470c-a34e-20552ea7ccf9.png)

### Alabasta
- 0.0.0.0/0 via 192.173.2.1

![image](https://user-images.githubusercontent.com/72689610/143669361-cc54ee1e-6ff5-4d5e-9622-aa52d9e23a9f.png)

###	OIMO
- 0.0.0.0/0 via 192.173.0.1
- 192.173.4.0/22 via 192.173.1.2

![image](https://user-images.githubusercontent.com/72689610/143669408-d69f65a4-09b5-4b1e-a70e-3c2f404effc4.png)

### Seastone
- 0.0.0.0/0 via 192.173.1.1

![image](https://user-images.githubusercontent.com/72689610/143669436-c829ae6a-10ed-433b-a5d0-3d41a9b8f384.png)

### Testing
Untuk testing sendiri dapat dilakukan dengan cara berikut :
1. Klik Menu `Add Simple PDU`
2. Pilih Source
3. Pilih Destination
4. Cek apakah ping tersebut success atau tidak

Berikut adalah contohnya:

![Testing](https://user-images.githubusercontent.com/72689610/143669632-294cd1a7-8f8d-4b71-9a1b-afaba1150828.png)
