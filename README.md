# Proyek Sistem Informasi Cyber Cafe

Ini adalah aplikasi web full-stack yang dibangun menggunakan Laravel (PHP) untuk mengelola operasional Cyber Cafe. Aplikasi ini mencakup sistem pemesanan pelanggan (frontend) dan panel admin (backend) untuk manajemen.

## 🚀 Cara Menjalankan Proyek (How to Run)

Berikut adalah panduan langkah demi langkah untuk menginstal dan menjalankan proyek Cyber Cafe ini di lingkungan pengembangan lokal Anda.

### 1. Prasyarat

Pastikan komputer Anda telah terinstal perangkat lunak berikut:
* **XAMPP** (sebagai server Apache dan database MySQL/MariaDB)
* **Composer** (untuk manajemen dependensi PHP)
* **Git** (untuk meng-kloning repository)

---

### 2. Instalasi Proyek

1.  **Nyalakan XAMPP**
    Buka XAMPP Control Panel dan nyalakan modul **Apache** dan **MySQL**.

2.  **Kloning Repository**
    Buka terminal (Git Bash, CMD, atau PowerShell), masuk ke folder `htdocs` XAMPP Anda, dan kloning proyek ini:
    ```bash
    cd C:\xampp\htdocs
    git clone [https://github.com/livlinee/Penjaminan-Mutu-Sistem-Informasi_-SI_A_Kelompok-2.git](https://github.com/livlinee/Penjaminan-Mutu-Sistem-Informasi_-SI_A_Kelompok-2.git) Cyber_Cafe_new
    cd Cyber_Cafe_new
    ```

3.  **Instal Dependensi**
    Instal semua *package* PHP (seperti Laravel, Laravel Excel) menggunakan Composer:
    ```bash
    composer install
    ```

4.  **Siapkan File `.env`**
    Salin file `.env.example` menjadi `.env` baru, lalu buat kunci aplikasi:
    ```bash
    copy .env.example .env
    php artisan key:generate
    ```

5.  **Buat Database Kosong**
    * Buka browser dan pergi ke **`http://localhost/phpmyadmin`**.
    * Buat database baru dengan nama persis: **`cyber_cafe`**

6.  **Konfigurasi `.env`**
    Buka file `.env` yang baru Anda buat dan pastikan pengaturan database Anda sudah benar. (Pengaturan *default* XAMPP biasanya sudah benar).

    **Database:**
    ```env
    DB_CONNECTION=mysql
    DB_HOST=127.0.0.1
    DB_PORT=3306
    DB_DATABASE=cyber_cafe
    DB_USERNAME=root
    DB_PASSWORD=
    ```

    **Email:** (Wajib diisi agar fitur struk via email berfungsi)
    ```env
    MAIL_MAILER=smtp
    MAIL_HOST=smtp.gmail.com
    MAIL_PORT=465
    MAIL_USERNAME="email-anda@gmail.com"
    MAIL_PASSWORD="password-app-16-digit-dari-google"
    MAIL_ENCRYPTION=ssl
    MAIL_FROM_ADDRESS="email-anda@gmail.com"
    MAIL_FROM_NAME="${APP_NAME}"
    ```

7.  **Import Database (Langkah Kunci)**
    *Repository* ini sudah menyertakan file `.sql` berisi data. Anda tidak perlu menjalankan migrasi. Cukup impor file tersebut:
    * Di **phpMyAdmin**, klik database **`cyber_cafe`** yang baru Anda buat.
    * Klik tab **"Import"** di bagian atas.
    * Klik **"Choose File" (Pilih File)** dan temukan file `.sql` yang ada di dalam folder proyek Anda (misalnya: `cyber_cafe.sql`).
    * Scroll ke bawah dan klik **"Go"** atau **"Import"**.

    Ini akan membuat semua tabel (`admin`, `menu`, `transaksi`, dll.) dan mengisi data *default* (termasuk akun admin `tes`).

8.  **Jalankan Server**
    Terakhir, jalankan server pengembangan Laravel:
    ```bash
    php artisan serve
    ```

---

### 3. Mengakses Aplikasi

Setelah server berjalan, Anda bisa mengakses aplikasi:

* **Halaman Pelanggan (Frontend):**
    `http://localhost:8000`

* **Halaman Login Admin (Backend):**
    `http://localhost:8000/admin/login`

* **Kredensial Login Admin:**
    * Username: `tes`
    * Password: `tes`
