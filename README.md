# 🎂 Dad's Birthday Hub

Website kado kenangan digital interaktif untuk merayakan hari ulang tahun Ayah tercinta. Dirancang khusus dengan kenyamanan visual maksimal untuk smartphone Android (ukuran teks besar, kontras tajam Biru Navy & Emas, serta alur *single vertical scroll* tanpa menu rumit).

---

## 🌟 Fitur Utama (Sesuai PRD)

- **Cover & Buka Kado (FR-01, US-01):** Halaman awal yang bersih dan elegan dengan tombol "Buka Kado".
- **Visual & Tipografi Ramah Ayah (FR-02, US-02):** Font terbaca jelas (minimal 17px), kontras tinggi (Navy Blue `#071329` & Gold `#f6c445`), serta partikel emas melayang di latar belakang.
- **Scroll Fade-in Animation (FR-03, US-03):** Pesan, doa, dan kata-kata menyentuh muncul satu per satu dengan transisi halus saat layar digulir ke bawah menggunakan *Intersection Observer*.
- **Pemutar Musik Otomatis (FR-04, US-04):** Musik latar langsung berputar otomatis saat tombol "Buka Kado" ditekan.
  > *Catatan Cerdas: Jika file `bgm.mp3` belum dimasukkan, sistem secara otomatis memainkan melodi akustik instrumen hangat langsung dari browser (Web Audio API).*
- **Interaksi "Kirim Peluk Hangat":** Ayah atau keluarga dapat menyentuh tombol peluk untuk memunculkan efek hujan cinta dan doa melayang.

---

## 📂 Struktur File

```text
Dad's birthday Hub/
├── index.html        # Single-file HTML berisi seluruh kode, inline CSS & JavaScript
├── bgm.mp3           # (Opsional) File lagu latar lokal favorit Ayah (< 5MB)
└── README.md         # Dokumentasi & panduan deployment
```

---

## 🎵 Cara Menambahkan Lagu (`bgm.mp3`)

1. Siapkan file lagu kesukaan Ayah berformat `.mp3` (misalnya lagu instrumen hangat atau lagu kenangan).
2. Beri nama file tersebut: `bgm.mp3`.
3. Letakkan file `bgm.mp3` tepat di samping file `index.html` (di folder yang sama).
4. Selesai! Saat tombol "Buka Kado" diklik, lagu tersebut akan otomatis berputar.

---

## 📸 Cara Mengganti Foto Kenangan (Opsional)

Jika ingin mengganti foto keluarga:
1. Buka file `index.html` dengan text editor (seperti Notepad / VS Code).
2. Cari bagian `<!-- Foto Kenangan Hangat -->` atau cari tag `<img src="...">`.
3. Ganti URL tersebut dengan nama file foto lokal (contoh: `foto-ayah.jpg` yang ditaruh di folder yang sama) atau link foto lainnya.

---

## 🚀 Panduan Rilis ke GitHub Pages (Gratis / Rp0)

Web ini 100% statis (*zero backend*), sehingga bisa dihosting gratis di GitHub Pages dalam waktu kurang dari 2 menit:

1. **Buat Repository Baru di GitHub:**
   - Masuk ke akun GitHub Anda.
   - Klik **New Repository** (beri nama misalnya: `dads-birthday`).
   - Pilih **Public**, lalu klik **Create repository**.

2. **Upload File:**
   - Klik tombol **Upload files** pada repository GitHub.
   - Drag & drop file `index.html` dan `bgm.mp3`.
   - Klik **Commit changes**.

3. **Aktifkan GitHub Pages:**
   - Masuk ke tab **Settings** di repository tersebut.
   - Di bilah menu kiri, klik **Pages**.
   - Pada bagian **Branch**, pilih `main` (atau `master`) dan folder `/ (root)`, lalu klik **Save**.
   - Tunggu sekitar 1–2 menit, link website akan aktif (contoh: `https://username.github.io/dads-birthday/`).

4. **Bagikan ke Ayah:**
   - Kirim link tersebut ke WhatsApp Ayah pada hari ulang tahunnya. Ayah cukup membuka link dan menekan tombol **"Buka Kado"**!

