<p align="center">
    <a href="https://laravel.com" target="_blank">
        <img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo">
    </a>
</p>

<p align="center">
    <a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
    <a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
    <a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
    <a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

# Laravel 8 Project

Proyek ini adalah aplikasi web berbasis Laravel 8. Laravel adalah framework PHP yang kuat dan fleksibel, yang memungkinkan pengembangan aplikasi web dengan cepat dan mudah.

## Persyaratan Sistem

Sebelum menjalankan proyek ini, pastikan server atau mesin lokal Anda memenuhi persyaratan berikut:

- PHP >= 7.3
- Composer
- MySQL atau database lain yang didukung
- Ekstensi PHP yang diperlukan: OpenSSL, PDO, Mbstring, Tokenizer, XML, Ctype, JSON

## Instalasi

Ikuti langkah-langkah berikut untuk meng-clone dan menjalankan proyek Laravel ini di mesin lokal Anda:

### 1. Clone Repository

Clone repository dari GitHub ke mesin lokal Anda menggunakan perintah berikut:

        git clone https://github.com/username/repository.git
### 2. Masuk Folder Yang sudah di commit
        cd repository
### 3. Instal Dependensi
Instal semua dependensi PHP yang diperlukan menggunakan Composer:

        composer install
### 4. Konfigurasi File .env:
Salin file .env.example menjadi .env:
        
        cp .env.example .env
Kemudian, buka file .env dan sesuaikan konfigurasi database sesuai dengan pengaturan lokal Anda:
        
        DB_DATABASE=nama_database
        DB_USERNAME=user_database
        DB_PASSWORD=password_database
### 5. Generate Application Key
Jalankan perintah berikut untuk menghasilkan application key:

        php artisan key:generate
### 6.5. Migrasi Database
Jalankan migrasi untuk membuat tabel di database:

        php artisan migrate

### 7.  Menjalankan Aplikasi
Jalankan server pengembangan Laravel menggunakan perintah berikut:

        php artisan serve
Akses aplikasi di browser Anda melalui URL http://localhost:8000.

Mengatasi Error
Jika Anda mengalami error seperti ini:

        PHP Warning:  require(C:\xampp\htdocs\repository/vendor/autoload.php): failed to open stream: No such file or directory in C:\xampp\htdocs\repository\artisan on line 18
Ini biasanya terjadi karena Composer belum diinstal atau Anda belum menjalankan `composer install`. Pastikan Composer telah terinstal dengan benar dan Anda telah menjalankan perintah `composer install` di direktori proyek.

Struktur Direktori Laravel
Berikut adalah beberapa direktori utama dalam proyek Laravel dan fungsinya:


## Struktur Direktori Laravel

Berikut adalah beberapa direktori utama dalam proyek Laravel dan fungsinya:

- **app/**  
  Berisi logika aplikasi termasuk model, controller, dan lainnya.

- **bootstrap/**  
  Berisi file yang memulai framework.

- **config/**  
  Berisi file konfigurasi untuk aplikasi.

- **database/**  
  Berisi file migrasi, seeder, dan pengaturan database lainnya.

- **public/**  
  Direktori yang dapat diakses secara publik, berisi file `index.php`.

- **resources/**  
  Berisi view, bahasa, dan aset yang digunakan oleh aplikasi.

- **routes/**  
  Berisi file rute aplikasi.

- **storage/**  
  Berisi file log, cache, dan file lain yang diperlukan.

- **tests/**  
  Berisi file tes unit dan fungsional.

- **vendor/**  
  Berisi dependensi pihak ketiga yang diinstal melalui Composer.




