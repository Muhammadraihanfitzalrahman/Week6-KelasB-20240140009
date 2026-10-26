# NusaMart - Katalog Produk & Pendaftaran Member (Tugas Fetch API & Form DOM / Event Handling)

Dua halaman statis (HTML + CSS + JavaScript native, tanpa library) yang dihubungkan lewat navigasi.

## Tampilan Aplikasi
## index.html
<img width="960" height="540" alt="Cuplikan layar 2026-10-26 200838" src="https://github.com/user-attachments/assets/df68e378-d332-4e4b-9531-74cde622e727" />
<img width="960" height="540" alt="Cuplikan layar 2026-10-26 200824" src="https://github.com/user-attachments/assets/c4767855-c539-47fa-8ea9-fa1591d41847" />

## form.html
<img width="960" height="540" alt="Cuplikan layar 2026-10-26 200913" src="https://github.com/user-attachments/assets/0e7b3417-2d67-4eb3-ad58-cf8e93331722" />
<img width="960" height="540" alt="Cuplikan layar 2026-10-26 201138" src="https://github.com/user-attachments/assets/6394905c-ec46-4266-b9d9-359d765b3393" />


## Fitur

### 1. Katalog Produk (`index.html`) - Fetch API
- Mengambil data dari `https://dummyjson.com/products` dengan `fetch()`.
- Menampilkan nama, harga, kategori, dan gambar produk lewat DOM.
- Status **loading** saat data diambil, pesan **error** + tombol "Coba lagi" bila gagal.
- Cek `response.ok` agar status 404/500 juga dianggap error.
- Pencarian produk (nama / kategori) memakai event `input`.

### 2. Pendaftaran Member (`form.html`) - DOM & Event Handling
- Kolom: nama, email, password, konfirmasi password, minat, persetujuan.
- Event: `input`, `blur`, `change`, `click`, `submit`, `reset`.
- Validasi langsung saat mengetik, pesan error muncul di bawah kolom.
- Indikator kekuatan password, tombol tampilkan/sembunyikan password.
- Hasil pendaftaran tampil dinamis sebagai kartu ringkasan.

| Kolom | Aturan |
|---|---|
| Nama | wajib, minimal 3 karakter, hanya huruf dan spasi |
| Email | wajib, format email valid |
| Password | wajib, minimal 8 karakter, mengandung huruf dan angka |
| Konfirmasi | wajib, sama dengan password |
| Persetujuan | wajib dicentang |

## Struktur Folder

```
tugas-fetch-form/
├── index.html
├── form.html
├── css/
│   ├── style.css
│   └── form.css
├── js/
│   ├── products.js
│   └── form.js
├── assets/
│   ├── favicon.svg
└── README.md
```

## Cara Menjalankan

Buka `index.html` di browser. Halaman produk membutuhkan koneksi internet.
