# 🎹 Khalid's Piano — Virtual Web Piano

[![Website](https://img.shields.io/badge/Live%20Demo-pianoku.web.id-brightgreen?style=for-the-badge&logo=cloudflare&logoColor=white)](https://pianoku.web.id)
[![Tech Stack](https://img.shields.io/badge/Stack-HTML5%20%7C%20CSS3%20%7C%20JS-blue?style=for-the-badge&logo=javascript)](https://pianoku.web.id)
[![Hosting](https://img.shields.io/badge/Hosted%20on-Cloudflare%20Pages-orange?style=for-the-badge&logo=cloudflare)](https://pianoku.web.id)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](LICENSE)

Aplikasi piano virtual interaktif berbasis web yang sangat ringan, responsif, dan dapat langsung dimainkan tanpa delay. Proyek ini dibangun sepenuhnya menggunakan **Vanilla HTML, CSS, dan JavaScript** tanpa library eksternal, memanfaatkan **Web Audio API** untuk menghasilkan suara secara sintetis (real-time). 

Website ini di-deploy secara gratis menggunakan infrastruktur **Cloudflare Pages** dengan custom domain pribadi di [pianoku.web.id](https://pianoku.web.id).

---

## ✨ Fitur Utama

- ⚡ **Tanpa Asset Audio Eksternal (Zero Latency):** Menggunakan **Web Audio API** bawaan browser untuk mensintesis suara secara langsung. Tidak perlu mengunduh file `.mp3` atau `.wav`, membuat aplikasi ini sangat ringan (ukuran total hanya sekitar **20 KB**) dan bebas delay.
- 🎵 **Pilihan Jenis Suara & Efek Lucu:**
  - Suara standar: *Piano (Sine)*, *Square*, *Sawtooth*, dan *Triangle*.
  - Suara lucu: *Kodok* 🐸, *Ayam* 🐔, *Bebek* 🦆, dan *Pistol* 🔫.
- 🎹 **Kontrol Oktaf & Volume:** Ganti oktaf dengan mudah (*C3*, *C4*, *C5*) dan atur volume suara langsung dari antarmuka pengguna.
- ⌨️ **Dukungan Keyboard PC/Laptop:**
  - **Tuts Putih:** `A`, `S`, `D`, `F`, `G`, `H`, `J`, `K`
  - **Tuts Hitam:** `W`, `E`, `T`, `Y`, `U`
- 🎲 **Fitur Random Play:** Menekan tombol keyboard lain di luar tuts di atas akan membunyikan tuts piano secara acak untuk eksperimen suara yang menyenangkan!
- 📱 **Desain Super Responsif & Estetis:** Menggunakan palet warna gelap yang elegan (*dark mode*), lengkap dengan efek transisi, bayangan dinamis, dan ukuran tuts yang otomatis menyesuaikan layar komputer, tablet, hingga smartphone (seperti Samsung S21 FE).
- 🏷️ **Petunjuk Tombol (Key Hints):** Opsi untuk menampilkan atau menyembunyikan label tombol keyboard di atas tuts piano.

---

## 🛠️ Teknologi yang Digunakan

1. **HTML5:** Struktur semantik untuk aplikasi web satu halaman (Single Page Application).
2. **CSS3 (Vanilla):** Styling kustom modern dengan efek bayangan, gradasi warna, efek hover, serta *media queries* untuk responsivitas maksimal di berbagai resolusi layar.
3. **JavaScript (ES6):**
   - **Web Audio API** untuk pembuatan osilator suara secara *real-time*.
   - Event Listener untuk *mouse pointer*, *touchscreen* (ponsel), dan *keyboard* fisik.
4. **Cloudflare Pages:** Untuk hosting web statis gratis berkinerja tinggi yang terintegrasi langsung dengan repository GitHub.

---

## 🚀 Cara Menjalankan secara Lokal

Karena proyek ini sepenuhnya statis (*static website*) dan hanya terdiri dari satu file `index.html`, Anda tidak perlu melakukan instalasi dependensi apa pun.

1. Clone repository ini ke komputer Anda:
   ```bash
   git clone https://github.com/username/nama-repo.git
   ```
2. Masuk ke direktori proyek:
   ```bash
   cd nama-repo
   ```
3. Buka file [index.html](file:///Users/barrukurniawan/Documents/piano/index.html) menggunakan browser kesayangan Anda (Chrome, Firefox, Safari, Edge, dll.).
   - Cukup klik dua kali pada file `index.html` atau jalankan local server jika diperlukan.

---

## 🌐 Panduan Deploy ke Cloudflare Pages (Gratis + Custom Domain)

Aplikasi ini dideploy ke **Cloudflare Pages** secara gratis dengan langkah-langkah mudah berikut:

### 1. Persiapan di GitHub
Pastikan file `index.html` berada di root repository GitHub Anda.

### 2. Konfigurasi di Cloudflare
1. Masuk ke dashboard [Cloudflare](https://dash.cloudflare.com/).
2. Navigasi ke menu **Workers & Pages** -> **Create application** -> **Pages** -> **Connect to Git**.
3. Pilih repository GitHub Anda.
4. Pada bagian **Build settings**:
   - **Framework preset:** `None`
   - **Build command:** *Biarkan kosong*
   - **Build output directory:** `.` (atau biarkan kosong jika defaultnya adalah root)
5. Klik **Save and Deploy**. Cloudflare akan membuild proyek Anda dalam beberapa detik.

### 3. Mengatur Custom Domain (`pianoku.web.id`)
1. Setelah berhasil dideploy, buka tab **Custom domains** pada halaman proyek Pages Anda di Cloudflare.
2. Klik **Set up a custom domain** dan masukkan `pianoku.web.id`.
3. Cloudflare akan secara otomatis memperbarui DNS record di akun Cloudflare Anda untuk mengarahkan domain tersebut ke aplikasi Pages.
4. Tunggu sertifikat SSL aktif secara otomatis. Selesai! Proyek Anda kini bisa diakses secara publik dan aman via HTTPS.

---

## 📄 Lisensi

Proyek ini dilisensikan di bawah **MIT License** - lihat file [LICENSE](LICENSE) untuk detail lebih lanjut.

---

*Dibuat dengan 💖 oleh Khalid. Selamat bermain musik! 🎶*
