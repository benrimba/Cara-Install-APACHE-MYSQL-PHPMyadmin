# Cara Install APACHE, MYSQL dan PHPMyadmin Linux Ubuntu 20.04

#### Langkah 1 : Update Server
###### ```sudo apt-get update```
#### Langkah 2 : Install Apache
###### ```sudo apt-get install apache2 ``` tunggu sampai selesai
#### Setting mod_rewrite Apache
###### ```sudo nano /etc/apache2/sites-available/000-default.conf```
###### Cari baris kode
###### ```php DocumentRoot /var/www/html ```
###### Setelah proses install Apache selesai, Anda perlu mengecek apakah instalasi berhasil atau tidak. Anda bisa mengeceknya dengan membuka IP server Anda seperti ini:
###### ```http://localhost/ ```
#### Langkah 3 : Install MySQL v.8
###### ```sudo apt-get install mysql-server```
###### ```sudo mysql_secure_installation```
#### Merubah Password MySQL v.8
###### Masuk Ke Mysql dengan Perintah ```sudo mysql```
###### mysql>```ALTER USER 'root'@'localhost' IDENTIFIED BY 'NewPassword';```
#### Langkah 4 : Install PHP
###### ``` sudo apt-get install php php-mysql libapache2-mod-php php-cli php-cgi php-gd mysql-server mysql-client zip -y ```
###### setelah selesai install, untuk memastikan berhasil atau tidaknya kita masuk ke direktori installnnya terlebih dahulu
###### ```cd /var/www/html```
###### ```sudo touch info.php```
###### ```sudo nano info.php```
###### ```php <?php phpinfo(); ?>```
###### Kemudian save dengan klik CTRL+X lalu tekan y dan ENTER
###### Jika file info PHP sudah ditambahkan,  masukkan perintah berikut di web browser Anda untuk cek apakah  instalasi PHP berhasil atau tidak.
#### Langkah 5 : Install phpMyAdmin
###### ```sudo apt-get install phpmyadmin```

