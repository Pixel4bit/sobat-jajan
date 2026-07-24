# 🍿 Sobat Jajan - Katalog & Pricelist Jajanan SPA

Aplikasi web satu halaman (*Single Page Application*) katalog dan *pricelist* jajanan rumahan buatan **Sobat Jajan**. Dibangun secara terintegrasi dalam **satu file HTML** (*All-in-One SPA*) tanpa perlu instalasi *backend* atau server khusus.

---

## ✨ Fitur Utama

### 🛒 Tampilan Pelanggan (Customer View)
* **Katalog Interaktif:** Menampilkan berbagai pilihan jajanan, gramasi, dan harga secara dinamis.
* **Filter & Pencarian:** Cari jajanan favorit dengan mudah melalui *search bar*.
* **Order via WhatsApp:** Pemesanan otomatis diformat menjadi pesan WhatsApp yang siap dikirim.
* **Request Jajanan Custom:** Pengunjung bisa melayangkan permintaan jajanan yang belum ada di katalog via WhatsApp.
* **Informasi Cara Bayar & QRIS:** Menampilkan langkah pemesanan dan kode QRIS pembayaran yang bisa diunduh (*download*).

### ⚙️ Panel Admin Tersembunyi (Hidden Admin Panel)
* **Akses Aksesibilitas:** Tombol rahasia di *footer* untuk masuk ke Panel Admin dengan kata sandi.
* **Manajemen Produk (CRUD):** Tambah, edit, atau hapus produk dan varian gramasi/harga.
* **Kustomisasi Template Pesan:** Atur format pesan WhatsApp untuk order dan *request* produk.
* **Pengaturan QRIS & Kontak:** Unggah gambar QRIS baru dan perbarui nomor WhatsApp tujuan.
* **Ekspor & Impor Data:** Cadangkan (*backup*) atau pulihkan (*restore*) seluruh database produk dan pengaturan dalam format `.json`.

---

## 🛠️ Tumpukan Teknologi (Tech Stack)

* **HTML5** — Struktur mark-up halaman.
* **Tailwind CSS (via CDN)** — Styling antarmuka yang modern, responsif, dan fleksibel.
* **Vanilla JavaScript (ES6+)** — Logika aplikasi, manipulasi DOM, dan pengelolaan status.
* **IndexedDB** — Penyimpanan database lokal di browser (menyimpan data produk, konfigurasi, dan QRIS sebagai base64).

---

## 🚀 Cara Menjalankan Aplikasi

Aplikasi ini tidak membutuhkan *framework*, *Node.js*, atau proses kompilasi (*build process*).

1. Clone repositori ini:
   ```bash
   git clone https://github.com/username/sobat-jajan.git
   ```
2. Buka folder proyek dan jalankan file `index.html` langsung di browser favorit Anda, atau gunakan ekstensi seperti **Live Server** di VS Code.

---

## 🔑 Akses Admin Panel Default

* **Cara Buka:** Klik simbol titik-titik `••••` pada bagian *footer* (samping teks *Copyright*).
* **Password Default:** Masukkan password sesuai konfigurasi di skrip utama (`adminPassword`).

---

## 📁 Struktur Kode (`index.html`)

Aplikasi ini dikelompokkan ke dalam beberapa bagian utama di dalam satu file:

1. **Tailwind Config & Custom Style** — Pengaturan warna tema dan animasi.
2. **Markup Visual** — Header/Hero, Katalog Produk, Cara Pesan, QRIS, dan Footer.
3. **Modals** — Modal Request Jajan & Modal Admin Panel.
4. **Data Layer (IndexedDB)** — Fungsi pembantu CRUD ke database lokal browser.
5. **State & Logic** — Logika render dinamis, integrasi WhatsApp, dan manajemen tab admin.

---

## 📄 Lisensi

Proyek ini dirilis di bawah lisensi **MIT License**.
