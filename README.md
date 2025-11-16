# Aplikasi Analisis Artikel

Selamat datang di Aplikasi Analisis Artikel! Aplikasi web ini dibangun menggunakan Laravel dan dirancang untuk menyediakan alat bantu analisis teks yang sederhana namun kuat. Antarmukanya yang bersih dan modern dibuat dengan Tailwind CSS, memastikan pengalaman pengguna yang responsif dan menyenangkan di semua perangkat.

## ✨ Fitur Utama

Aplikasi ini dilengkapi dengan tiga fitur analisis utama:

1.  **Pencarian Kata**: Hitung frekuensi kemunculan sebuah kata dalam artikel. Masukkan kata yang ingin Anda cari, dan aplikasi akan menampilkan berapa kali kata tersebut ditemukan.

2.  **Penggantian Kata**: Ganti sebuah kata dalam artikel dengan kata lain. Fitur ini akan mencari semua kemunculan kata target dan menggantinya dengan kata baru yang Anda berikan, lalu menampilkan hasilnya secara visual.

3.  **Pengurutan Kata**: Ekstrak semua kata unik dari artikel dan tampilkan dalam urutan abjad (A-Z). Hasilnya disajikan dalam format "tag" atau "bubble" yang rapi dan mudah dibaca.

## 🚀 Teknologi yang Digunakan

-   **Backend**: PHP 8+ dengan framework Laravel 10
-   **Frontend**: Blade, Tailwind CSS
-   **Lingkungan Pengembangan**: Dikonfigurasi untuk Firebase Studio (Project IDX)

## 🛠️ Panduan Instalasi dan Penggunaan

Ikuti langkah-langkah berikut untuk menjalankan aplikasi ini di lingkungan pengembangan lokal Anda.

### 1. Prasyarat

Pastikan Anda memiliki perangkat lunak berikut terinstal:
-   PHP >= 8.1
-   Composer
-   Node.js & npm

### 2. Instalasi

```bash
# 1. Clone repositori ini

# 2. Masuk ke direktori proyek

# 3. Instal dependensi PHP
composer install

# 4. Instal dependensi Node.js
npm install

# 5. Salin file environment dan buat kunci aplikasi
cp .env.example .env
php artisan key:generate
```

### 3. Menjalankan Aplikasi

Untuk memulai server pengembangan, jalankan perintah berikut:

```bash
php artisan serve
```

Setelah server berjalan, buka browser Anda dan akses aplikasi di alamat:
[**http://127.0.0.1:8000**](http://127.0.0.1:8000)

## 📄 Struktur Proyek

-   **Controller Utama**: Logika aplikasi berada di `app/Http/Controllers/ArticleController.php`.
-   **Rute**: Semua rute didefinisikan dalam `routes/web.php`.
-   **Tampilan**: Antarmuka pengguna utama terletak di `resources/views/artikel/index.blade.php`.
-   **Teks Artikel**: Teks asli untuk dianalisis disimpan langsung di dalam `ArticleController`.
