# Jarkom-Modul-4-B08-2021

Nama | NRP |
--- | --- | 
Adam Hadi Prasetyo | 05111940000224 |
Vyra Fania Adelina | 05111940000109 |
Tsania Az Zahra | 05111940000032 |



PENGERJAAN SUBNETTING DAN ROUTING PADA CISCO PACKET TRACER


3. Meng-assign Subnet Mask Pada Tiap Subnet Berdasarkan Kebutuhan Host dan IP Address nya Masing-masing

Subnet |	Jumlah Host Netmask |	Netmask |	Subnet Mask |	IP |
--- | ---| ---| ---| ---|
A1 |	128 |	/25 |	255.255.255.128 | (256-128=128)	10.11.27.0 |
A2 | 2048 |	/21 |	255.255.248.0(256-2048=1792) Pinjam 3 Digit Dari Oktet Ketiga Jadi Oktet Ketiga Sisanya = 2^8-2^3=248. |	10.11.1.0 |
A3 |	1024 |	/22 |	255.255.252.0(256-1024==768) Pinjam 2 Digit Dari Oktet Ketiga Jadi Oktet Ketiga Sisanya = 252 |	10.11.8.0 |
A4 |	4 |	/30 |	255.255.255.252(256-4=252) |	10.11.27.144 |
A5 |	1024 |	/22 |	255.255.252.0 (Sama Seperti A3) |	10.11.16.0 |
A6 |	4 |	/30 |	255.255.255.252 (Sama Seperti A4) |	10.11.27.148 |
A7 |	1024 |	/22 |	255.255.252.0 (Sama Seperti A5) |	10.11.12.0 |
A8 |	512 |	/23 |	255.255.254.0 (256-512=256) Pinjam 1 Digit Dari Oktet Ketiga Jadi Oktet Ketiga Sisanya 254 |	10.11.26.0 |
A9 |	1024 |	/22 |	255.255.255.252(256-1024=768) Pinjam 2 Digit Dari Oktet Ketiga Jadi Oktet Ketiga Sisanya 252 |	10.11.20.0 |
A10 |	4 |	/30 |	255.255.255.252 (256-4=252) |	10.11.27.160 |
A11 |	512 |	/23 |	255.255.254.0 (Sama Seperti A8) |	10.11.24.0 |
A12 |	4 |	/30 |	255.255.255.252 (Sama Seperti A10) |	10.11.27.164 |
A13 |	16 |	/28 |	255.255.255.240 (256-16=240) |	10.11.27.128 |
A14 |	4 |	/30 |	255.255.255.252 (Sama Seperti A10) |	10.11.27.152 |
A15 |	4 |	/30 |	255.255.255.252 (Sama Seperti A10) |	10.11.27.156 |

4. Menentukan IP Network

Total Host : 
5834 -> 10.11.0.0/19 (8192 Host) → CUKUP!

IP Network : 10.11.0.0

5. Mengkonfigurasikan IP Address Tiap Host dan Router Berdasarkan Poin Sebelumnya
Contoh; Konfigurasi IP Address dan Subnet Mask Pada Foosha:
- Pada Jaringan Ethernet Jalur 0/0 yang Terhubung Dengan Switch dan Server DORIKI
![image](https://user-images.githubusercontent.com/69724694/143685281-ed86c4c5-c658-4d01-abf2-5ad3f190aaca.png)
- Assignment IP Address Ini Dilakukan Di Seluruh Host dan Router
6. Mengaplikasikan Routing Agar Seluruh Subnet Dapat Saling Terhubung Dengan Acuan Host Ideal Yaitu Foosha
- Dikarenakan Foosha Tidak Terhubung Langsung Dengan Sebagian Subnet yang Ada Pada Jaringan Maka Dibutuhkan Adanya Perantara Diantara Foosha dan Subnet yang Dimaksud. Maka Digunakan Routing Sebagai Cara Untuk Menghubungkan Foosha dan Subnet-Subnet Jauh Yang Lain.
- Contoh; Konfigurasi Routing Pada Foosha Terhadap Subnet-Subnet Yang Melalui Router GUANHAO
![image](https://user-images.githubusercontent.com/69724694/143685393-27fd4c29-f8e5-4f79-9b10-d76616426e78.png)
