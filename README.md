# Penjaminan Mutu Sistem Informasi_SI_A_Kelompok 2
**Judul Project:** Pemesanan Online Melalui QR Cafe  

**Tim Pengembang:**
1. **Project Manager:** Lila Vimala_F521230801  
2. **Database Administrator:** Nur Khalizah_F521230820  
3. **UI/UX Designer:** Cahya Nabila Mannassai_F521230823  
4. **Fullstack Developer:** Syahril Ramadhan_F521230838  
5. **Quality Assurance:** Desak Damayanti_F521230804  

---

## 📘 Deskripsi Aplikasi
Aplikasi **Pemesanan Online Melalui QR Cafe** merupakan sistem berbasis web yang memudahkan pelanggan untuk melakukan pemesanan makanan dan minuman secara digital melalui pemindaian QR Code di meja masing-masing.  

Sistem ini dirancang untuk meningkatkan efisiensi pelayanan di kafe dengan fitur seperti:
- Pemindaian QR untuk melihat menu
- Pemesanan langsung dari perangkat pelanggan
- Pengelolaan menu dan transaksi oleh admin

---

## ⚙️ Install / How to Run

### 1. Clone Repository
```bash
git clone https://github.com/livinee/Penjaminan-Mutu-Sistem-Informasi_SI_A_Kelompok-2.git
cd Penjaminan-Mutu-Sistem-Informasi_SI_A_Kelompok-2
composer install
cp .env.example .env
```

### 2. Konfigurasi Database
Buka file **.env** lalu ubah sesuai dengan database yang kamu gunakan:
```bash
DB_PORT=3306
DB_DATABASE=laravel
DB_USERNAME=root
DB_PASSWORD=
```

### 3. Instalasi Website
```bash
php artisan key:generate
php artisan migrate --seed
```

### 4. Jalankan Website
```bash
php artisan serve
```

Setelah server berjalan, buka browser dan akses:
```
http://localhost:8000
```

---

## 🎨 RANCANGAN UI/UX DI FIGMA
<p align="center">
  <img height="400" alt="1" src="https://github.com/user-attachments/assets/16863889-ebc7-4dbb-ac02-4378dd891439" />
  <img height="400" alt="2" src="https://github.com/user-attachments/assets/0224dd6c-c69a-473a-8191-314e92b25b9c" />
  <img height="400" alt="3" src="https://github.com/user-attachments/assets/4a2cf798-f969-4002-a2c0-179be0caed58" />
  <img height="400" alt="4" src="https://github.com/user-attachments/assets/48136acd-70fb-4aa2-8668-fc1624745b64" />
  <img height="400" alt="5" src="https://github.com/user-attachments/assets/2d1dccad-35b4-4aa5-a04b-39808081d667" />
  <img height="400" alt="6" src="https://github.com/user-attachments/assets/29b25359-3481-4a23-a096-c5dfdf841216" />
  <img height="400" alt="7" src="https://github.com/user-attachments/assets/7e6043ef-682d-416a-a8c5-a163a7a70464" />
  <img height="400" alt="8" src="https://github.com/user-attachments/assets/3723cbfb-c5ea-478f-b5b9-77e03be629ec" />
  <img height="400" alt="9" src="https://github.com/user-attachments/assets/e8584391-61e9-46f8-8db2-ba438e97feb3" />
  <img height="400" alt="10" src="https://github.com/user-attachments/assets/131dcfed-3c5f-4427-adae-968cd074b6b8" />
</p>

---

## 🧑‍💻 Lisensi
Proyek ini dilisensikan di bawah [MIT License](LICENSE).
