# Week6-KelasB-20240140009

Proyek Praktikum **Pengembangan Aplikasi Web (PAW)** - Pertemuan 6  
Repositori ini berisi implementasi aplikasi web **NusaMart**, platform e-commerce dan pendaftaran member interaktif berbasis HTML, CSS, dan JavaScript murni (Vanilla JS).

---

## 📌 Identitas Proyek

- **Nama Repositori**: `Week6-KelasB-20240140009`
- **NIM**: 20240140009
- **Kelas**: B
- **Topik**: Manipulasi DOM, Asynchronous JavaScript (Fetch API), Event Handling, Validasi Formulir, dan Styling Modern.

---

## 🚀 Fitur Utama

### 1. Halaman Belanja / Katalog Produk (`index.html`)
- **Integrasi REST API DummyJSON**: Mengambil data produk secara asinkronus menggunakan `fetch()` API.
- **Rendering Dinamis**: Menampilkan kartu produk lengkap dengan gambar thumbnail, judul, kategori, deskripsi, harga terformat ($), dan rating bintang.
- **Pencarian Real-Time**: Fitur pencarian instan berdasarkan nama produk atau kategori produk dengan update jumlah hasil pencarian secara langsung.
- **State Loading & Penanganan Error**: Menampilkan indikator loading saat data diambil serta pesan error ramah pengguna dengan tombol "Coba lagi" jika terjadi kegagalan jaringan.

### 2. Halaman Formulir Pendaftaran Member (`form.html`)
- **Validasi Input Client-Side Real-Time**:
  - **Nama Lengkap**: Wajib diisi, minimal 3 karakter, dan hanya boleh mengandung huruf/spasi.
  - **Email**: Format email tervalidasi menggunakan regex standar.
  - **Password**: Wajib diisi, minimal 8 karakter, serta harus mengombinasikan huruf dan angka.
  - **Konfirmasi Password**: Memastikan kecocokan data dengan kata sandi yang telah diisi.
  - **Persetujuan Ketentuan**: Validasi checkbox persetujuan syarat dan ketentuan.
- **Indikator Kekuatan Password (Password Strength Meter)**: Visualisasi bilah bar dinamis dan status level kekuatan password (Sangat Lemah, Cukup, Kuat, Sangat Kuat).
- **Toggle Lihat Password**: Fitur menampilkan/menyembunyikan teks password secara interaktif.
- **Kartu Ringkasan Pendaftaran**: Menampilkan data hasil registrasi dalam kartu profil ringkas setelah form berhasil divalidasi dan disubmit.

### 3. Fitur Global & Aksesibilitas
- **Dark Mode & Light Mode**: Switcher tema visual yang dapat beralih secara halus dan preferensi disimpan pada `localStorage` browser.
- **Desain Responsif**: Tampilan optimal pada berbagai resolusi perangkat (Desktop, Tablet, dan Mobile).
- **Semantik & Aksesibilitas**: Penggunaan elemen semantik HTML5, atribut `aria-live`, `aria-invalid`, serta navigasi ramah pembaca layar (screen reader).

---

## 📁 Struktur Direktori

```text
Pertemuan6_PAW/
├── assets/
│   └── favicon.svg       # Ikon logo NusaMart
├── css/
│   ├── style.css         # Styling sistem desain utama & katalog produk
│   ├── form.css          # Styling khusus formulir pendaftaran & indikator
│   └── from.css          # File pendukung kompatibilitas styling formulir
├── js/
│   ├── theme.js          # Logika toggle dark/light mode & localStorage
│   ├── products.js       # Integrasi fetch API DummyJSON, filter, & render produk
│   ├── form.js           # Validasi input formulir, password strength & submit
│   └── from.js           # File pendukung kompatibilitas logika formulir
├── form.html             # Halaman antarmuka pendaftaran member
├── index.html            # Halaman antarmuka katalog belanja produk
└── README.md             # Dokumentasi lengkap proyek
```

---

## 🛠️ Cara Menjalankan Proyek

1. **Clone Repositori**:
   ```bash
   git clone https://github.com/Muhammadraihanfitzalrahman/Week6-KelasB-20240140009.git
   ```
2. **Masuk ke Direktori Proyek**:
   ```bash
   cd Week6-KelasB-20240140009
   ```
3. **Buka Menggunakan Browser atau Web Server Lokal**:
   - Klik ganda berkas `index.html` untuk langsung membuka halaman di peramban web, **atau**
   - Gunakan ekstensi **VS Code Live Server** / server statis lokal:
     ```bash
     npx serve .
     ```
   - Buka `http://localhost:3000` atau URL lokal yang disediakan.
