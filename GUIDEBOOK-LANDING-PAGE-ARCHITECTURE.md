# Spesifikasi Arsitektur Halaman Guidebook Interaktif AIdah
**Dokumen Perencanaan Desain, Konten, & Implementasi**
*Domain:* `https://aidah.web.id/guidebook`  
*Repo:* `/home/hermes/landingpage-aidah/src/pages/guidebook.astro`  
*Target Rilis:* Web Landing Page Publik & Terintegrasi ke Aplikasi AIdah (Web & Mobile)

---

## 1. Latar Belakang & Tujuan
Aplikasi **AIdah** memiliki fitur finansial yang kaya dan unik: asisten chat berbasis Natural Language Processing (Nemo AI), pemindai struk belanja dengan Vision AI, sistem *carry-over* saldo multi-bulan, alokasi tabungan impian, budget anti-bocor, laporan analitik mingguan, hingga proteksi keamanan setara perbankan (*Auto-Lock PIN saat keluar aplikasi*).

Halaman **Guidebook** ini dirancang sebagai pusat panduan visual interaktif lengkap (bukan sekadar teks dokumentasi kaku) yang membantu pengguna baru maupun pengguna aktif menguasai seluruh fitur AIdah dalam hitungan menit, sekaligus menjadi sarana edukasi calon pengguna yang ingin memahami cara kerja aplikasi sebelum mendaftar.

---

## 2. Prinsip Desain & Visual
1. **Neo-brutalism Playful & Clean**:
   - Border tegas `2px solid var(--ink)` (`#1a1a1a`), sudut membulat proporsional (`14px` - `20px`), dan bayangan tebal `box-shadow: 4px 4px 0 var(--ink)`.
   - Palet warna konsisten: Biru Royal (`#3B82F6`), Nemo Orange (`#F97316`), Emerald Green (`#10B981`), Pastel Soft Backgrounds (`#EFF6FF`, `#F0FDF4`, `#FFF7ED`).
2. **Copywriting Langsung, Tegas, & Percaya Diri**:
   - Menghindari kata ragu-ragu seperti *"seikhlasnya"* — menggunakan penegasan *"Akses Penuh Tanpa Batas dengan Traktir Kopi via QRIS"*.
   - Kalimat jelas, ringkas, informatif, dan langsung ke inti solusi.
3. **Navigasi Cepat (Quick Jump & Live Filter)**:
   - Header bar sticky dengan filter modul (Pencatatan Chat, Scan Struk, Saldo & Budget, Tabungan Impian, Laporan, Keamanan PIN).
   - Kolom pencarian instan (Live Search) untuk menemukan instruksi dalam 1 detik.
4. **Simulator Interaktif**:
   - Terdapat playground mini chat interaktif untuk mencoba simulasi mengetik pesan ke Nemo AI.

---

## 3. Struktur Konten & Modul Pembahasan

### Hero Section
* **Badge**: `📖 Panduan Resmi Penggunaan AIdah`
* **Heading**: *Kuasai Seluruh Fitur Finansialmu dalam Hitungan Menit*
* **Subheading**: *Panduan langkah demi langkah menggunakan asisten AI Nemo, memindai struk, mengatur limit pos belanja, menabung impian, hingga mengamankan aplikasi seperti mobile banking.*
* **Pencarian Cepat**: Input pencarian interaktif untuk menyaring topik panduan.
* **Aksi Cepat**: Tombol *Mulai Pakai Web* & *Download APK Android*.

---

### Modul 1: Memulai & Pengaturan Akun
* **Pendaftaran Akun Baru**:
  * Cara mendaftar dengan email dan password kuat (min. 8 karakter, huruf kapital, angka, simbol).
  * Verifikasi akun dan login cepat.
* **Setup Profil Awal**:
  * Memilih avatar emoji favorit (`🐟`, `🦁`, `🐱`, `🐶`, `🦊`, `🐼`, dll).
  * Memasukkan estimasi gaji bulanan rutin agar fitur persentase budget dan alokasi otomatis aktif optimal.
* **Masa Uji Coba 7 Hari & Perpanjangan**:
  * Cara kerja masa trial gratis 7 hari penuh tanpa kartu kredit.
  * Cara memperpanjang akses dengan traktir kopi via scan QRIS satu kali per 30 hari.

---

### Modul 2: Asisten Nemo AI — Pencatatan Bahasa Natural
* **Konsep Dasar**: Tidak perlu mengisi form bertingkat atau memilih dropdown rumit. Ketik seperti mengirim pesan WhatsApp ke teman.
* **Cheatsheet Kalimat Contoh**:
  * **Pengeluaran**:
    * `"kopi kenangan 24rb"` ➔ Pos Makan & Minum
    * `"bensin pertalite 50k"` ➔ Pos Transportasi
    * `"beli kuota internet telkomsel 100rb"` ➔ Pos Tagihan & Utilitas
  * **Pemasukan**:
    * `"gaji bulanan masuk 8jt"` ➔ Pos Pemasukan Gaji
    * `"dapat transferan freelance 1.5jt"` ➔ Pos Pemasukan Lainnya
  * **Tagihan Rutin Otomatis (Recurring)**:
    * Cara mencatat langganan bulanan: cukup centang/pilih opsi rutin agar sistem otomatis menjadwalkan jatuh tempo berikutnya.
* **Koreksi & Pembatalan Transaksi**:
  * Cara mengklik tombol edit (`✏️`) atau hapus (`×`) jika salah mengetik nominal.

---

### Modul 3: Pindai Struk Belanja Cerdas (Vision AI)
* **Langkah Menggunakan Kamera Struk**:
  * Buka tab chat Nemo ➔ Ketuk ikon kamera (`📷`).
  * Pilih ambil foto langsung atau unggah dari galeri.
* **Tips Foto Struk Agar Akurat**:
  * Pastikan pencahayaan cukup dan teks kasir tidak terlipat.
  * Letakkan struk di atas permukaan datar yang kontras.
* **Proses Review Cepat**:
  * AI mendeteksi nama merchant (Indomaret, Alfamart, Superindo, dsb), rincian item, dan total bayar.
  * Pengguna dapat memilih kategori secara massal (*bulk category*) atau per item sebelum menekan tombol simpan.

---

### Modul 4: Dashboard Saldo & Kontrol Privasi
* **Formula Saldo Total (Carry-over)**:
  * Penjelasan transparan bagaimana saldo bulan lalu yang tersisa otomatis digabungkan dengan mutasi bulan berjalan.
* **Fitur Sembunyikan Saldo (Toggle Mata 👁️)**:
  * Mengaburkan nominal saldo menjadi `••••••••` saat berada di tempat umum atau transportasi publik agar privasi terjaga.
* **Budget Alerts (Peringatan Anti-Bocor)**:
  * Indikator warna kuning (warning saat ≥80%) dan merah (over budget saat ≥100%) langsung di beranda.

---

### Modul 5: Batas Anggaran (Budget Anti-Bocor) & Kategori Kustom
* **Menetapkan Limit Pengeluaran**:
  * Menentukan batas maksimal untuk pos Makan, Belanja, Hiburan, dll.
* **Membuat Kategori Kustom**:
  * Cara menambah kategori baru lengkap dengan nama dan ikon emoji kustom.
* **Audit & Deduplikasi Kategori**:
  * Fitur pintar AIdah yang secara otomatis mencegah kategori kembar/duplikat.

---

### Modul 6: Tabungan Impian (Financial Goals)
* **Membuat Target Tabungan**:
  * Menentukan nama impian (contoh: *Upgrade Laptop*, *Liburan Bali*, *Dana Darurat*), target nominal, dan tanggal target.
* **Alokasi Sumber Dana Fleksibel**:
  * Pilihan menyisihkan uang dari *Saldo Bulan Ini* atau dari *Sisa Bulan Lalu*.
* **Pencatatan Tanpa Saldo Ganda**:
  * Uang yang dialokasikan ke impian otomatis tercatat agar saldo operasional tidak terpakai secara tidak sengaja.

---

### Modul 7: Laporan Keuangan (Cuan Report) & Ekspor Data
* **Analitik Mingguan (Weekly Breakdown W1–W4)**:
  * Mendeteksi minggu paling boros dalam satu bulan untuk evaluasi gaya hidup.
* **Grafik Tren 6 Bulan**:
  * Memantau kenaikan/penurunan pengeluaran jangka menengah.
* **Filter Waktu Cepat**:
  * Beralih dalam 1 klik antara filter *Hari Ini*, *7 Hari Terakhir*, *Bulan Ini*, dan *Semua*.
* **Ekspor Data**:
  * Ekspor transaksi ke format **CSV** (bisa dibuka di Excel/Google Sheets) dan format **PDF** untuk cetak/arsip.

---

### Modul 8: Fitur Keamanan Tingkat Tinggi (Mobile Banking Grade)
* **Kunci Otomatis (Auto-Lock on Background / App Close)**:
  * Setiap kali aplikasi ditutup, diminimalkan, atau layar HP mati, aplikasi otomatis terkunci seketika.
* **Buka Kunci Cepat dengan Biometrik**:
  * Integrasi sensor Sidik Jari (Fingerprint) & Face ID lokal.
* **Proteksi Lupa PIN & Reset Aman**:
  * Solusi pemulihan akun tanpa risiko kebocoran data.
* **Isolasi Data Database**:
  * Seluruh data transaksi dilindungi PostgreSQL Row Level Security (RLS) unik per User ID.

---

### Modul 9: Panduan Instalasi Aplikasi (Android & iOS)
* **Android (APK Standalone)**:
  * Cara download file installer APK (`app.aidah.web.id/api/download-apk`).
  * Cara mengizinkan instalasi dari browser dan memasang aplikasi.
* **iPhone (PWA Safari)**:
  * Buka `app.aidah.web.id` di Safari ➔ Ketuk tombol *Share* ➔ Pilih *Add to Home Screen*.
* **Nada Pengingat Nemo Chime**:
  * Penjelasan pengingat harian jam 08:00, 12:00, dan 20:00 WIB.

---

### Modul 10: FAQ & Pusat Bantuan
* Tanya jawab seputar sinkronisasi data antar perangkat, reset data transaksi, dan tombol kontak WhatsApp Admin langsung.

---

## 4. Rute & Penempatan File
* **File Utama**: `/home/hermes/landingpage-aidah/src/pages/guidebook.astro`
* **URL Akses**: `https://aidah.web.id/guidebook`
* **Navigasi Navbar**: Tambahkan link `Guidebook 📖` di navbar `/home/hermes/landingpage-aidah/src/components/Navbar.astro`.
* **Tautan dari Web App**: Tambahkan tombol *"Buka Guidebook 📖"* di menu Pengaturan (`src/pages/settings.astro`) dan profil mobile (`mobile/app/(tabs)/profile.tsx`).

---

## 5. Rencana Eksekusi
1. Membuat halaman Astro `src/pages/guidebook.astro` di project `landingpage-aidah` dengan seluruh modul dan styling neo-brutalisme lengkap.
2. Memperbarui `Navbar.astro` dan `Footer.astro` agar terhubung ke `/guidebook`.
3. Menjalankan `npm run build` di `landingpage-aidah` untuk verifikasi tanpa error kompilasi.
4. Melakukan deploy Cloudflare Worker untuk `aidah.web.id` via `wrangler deploy`.
5. Menambahkan tombol shortcut Guidebook di halaman Pengaturan Web dan Mobile.
