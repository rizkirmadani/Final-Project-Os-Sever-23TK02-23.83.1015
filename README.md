# Final-Project-Os-Sever-23TK02-23.83.1015
**Nama:** Rizki Ramadani  
**NIM:** 23.83.1015
**Kelas:** 23TK02  
**Mata Kuliah:** OS SERVER dan SISTEM ADMIN 

## Daftar Isi
1. [Instalasi OPEN SSH SERVER](#1-instalasi-open-ssh-server)
2. [Instalasi MYSQL SERVER](#2-instalasi-mysql-server)
3. [Instalasi APACHE2](#3-instalasi-apache2)
4. [Instalasi DATABASE SERVER](#4-instalasi-database-server)
5. [Instalasi FAIL2BAN](#5-instalasi-fail2ban)

## 1.Instalasi OPEN SSH SERVER
**Langkah 1:** Lakukan Instalasi Paket SSH Server
```bash
sudo apt install openssh-server -y
```
**Langkah 2:** Mengaktifkan Layanan ssh server
```bash
sudo systemctl enable ssh
```
**Langkah 3:** Memulai Layanan SSH SERVER
```bash
sudo systemctl start ssh
```
**Langkah 4:** Cek ip ubuntu server
```bash
ip a
```
**Langkah 5:** Cek status ubuntu server
```bash
sudo systemctl status ssh
```
**Langkah 6:** config ssh server
```bash
Buka CMD pada windows,lakukan konfigurasi pada ubuntu dengan cara <ssh username ubuntu@ip address ubuntu server> contoh:ssh rizki@192.168.100.94
setelah itu ketik manual "yes" dan masukkan password ubuntu server
```
**Langkah 5:** cek configurasi
![image](https://github.com/user-attachments/assets/c66310fd-92df-40a9-ba15-9b1bd991b5cd)


## 2.Installasi MY-SQL SERVER
**Langkah 1:** Install mysql server dengan perintah
```bash
sudo apt install mysql-server -y
```
**Langkah 2:** Install tumpukan LAMP (Linux, Apache, MySQL, PHP) pada sistem operasi dengan perintah
```bash
sudo apt install php libapache2-mod-php phpmysql
```
**Langkah 3:** Membuka File Konfigurasi Direktori Apache dengan perintah
```bash
sudo nano /etc/apache2/mods-enabled/dir.conf
```
**Langkah 4:** Membuka file bernama “info.php” pada direktori var/www/html
```bash
sudo nano /var/www/html/info.php
```
-isikan dengan code dibawah
```bash
<?php

phpinfo ();

?>
```
**Langkah 5:** cek configurasi

contoh :192.168.100.94/info.php
![image](https://github.com/user-attachments/assets/21c9f25b-b07a-4ab2-85a1-5652c49994af)


## 3.Installasi APACHE2
**Langkah 1:** Perbarui daftar paket dengan perintah
```bash
sudo apt update
```
**Langkah 2:** Installasi apache 2 dengan perintah
```bash
sudo apt install apache2 -y
```
**Langkah 3:** Memulai layanan server apahe2 dengan perintah
```bash
sudo systemctl start apache2
```
**Langkah 4:** Lakukan pengecekan ip addres ubuntu server dengan perintah
```bash
ip a
```
**Langkah 5:** Buka pada browser google chrome pada windows dan ketikkan ip addres tadi “192.168.1.13”


contoh ip saya : 192.168.100.94
![image](https://github.com/user-attachments/assets/26d3e4a4-0ad9-4877-a0fc-808b3cea0310)
## 4.Installasi DATABASE SERVER
**Langkah 1:** Installasi paket mariadb
```bash
sudo apt update
```
**Langkah 2:** Untuk mengamankan installasi pilihan
```bash
sudo apt install apache2 -y
```
**Langkah 3:** Lakukan instalasi paket
![Screenshot 2024-12-01 163243](https://github.com/user-attachments/assets/b76c67db-137c-496f-a956-bfea6eef03cb)
![Screenshot 2024-12-01 163503](https://github.com/user-attachments/assets/5d17d87f-fb12-4e77-a1ba-ac711a32b41a)
![Screenshot 2024-12-01 163541](https://github.com/user-attachments/assets/4cb885c4-d2b8-4ada-ad8d-a383d59a13f4)
![Screenshot 2024-12-01 163557](https://github.com/user-attachments/assets/fe008325-bab0-4584-b228-5378e09bec08)

```bash
sudo systemctl start apache2
```
**Langkah 4:** Restart ulang layanan
```bash
ip a
```
**Langkah 5:** CEK KONFIGURASI Buka pada browser windows gogole chrome dan ketikkan <ip address ubuntu server/phpmyadmin/> cth:192.168.1.13/phpmyadmin/
![image](https://github.com/user-attachments/assets/37cd45b6-0272-4c70-a9cb-11da59038098)

## 5.Installasi fail2bn
**Langkah 1:** Instalasi fail2ban
```bash
sudo apt install fail2ban -y
```
**Langkah 2:** nyalakan 
```bash
sudo systemctl enable fail2ban
```
**Langkah 3:** jalankan
```bash
sudo systemctl start fail2ban
```
**Langkah 4:** check status
```bash
sudo systecmtl status fail2ban
```
![image](https://github.com/user-attachments/assets/8c80ce3a-8635-42e9-9ced-3c6e50b4c749)

