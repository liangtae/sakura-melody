# sakura-melody
🌸 Aplikasi single-file HTML untuk mencatat &amp; mengelola koleksi musik pribadi — rating gaya sakura, tag/genre, galeri foto, ekspor Excel/PDF, dark mode — semua tersimpan lokal tanpa backend.

# 🌸 Sakura Melody — Koleksi Musik Pribadi

Aplikasi web satu-halaman (single-file HTML) untuk mencatat, menilai, dan mengelola koleksi musik pribadi — lagu, album, atau soundtrack favorit — dengan nuansa visual bertema Jepang/sakura yang tenang dan sinematik. Semua data tersimpan lokal di browser, tanpa backend, tanpa akun, tanpa server.

![Made with HTML/CSS/JS](https://img.shields.io/badge/stack-HTML%20%7C%20CSS%20%7C%20JS-C9628F)
![No backend](https://img.shields.io/badge/backend-none%20(localStorage)-7C8B5D)
![License](https://img.shields.io/badge/license-MIT-C79A4B)

---

## ✨ Fitur

- **Katalog musik** — simpan judul, artis, album, jenis (lagu/album), catatan, dan status "sudah didengarkan".
- **Rating gaya sakura** — beri rating menggunakan ikon bunga sakura, bukan bintang biasa.
- **Tag & genre** — beri tag bebas dan genre (termasuk genre custom buatan sendiri) untuk tiap entri, lalu filter lewat chip dan tab.
- **Pencarian & pagination** — cari cepat lewat search box, jelajahi koleksi lewat grid berhalaman dengan navigasi nomor halaman.
- **Pin favorit** — sematkan lagu favorit agar mudah ditemukan.
- **Thumbnail & galeri foto** — unggah cover/thumbnail per lagu, tambahkan galeri foto (URL atau upload), lengkap dengan lightbox untuk melihat foto secara penuh.
- **Mode bulk** — pilih banyak entri sekaligus untuk aksi massal.
- **Draf otomatis** — form tambah/edit lagu tersimpan otomatis sebagai draf sehingga tidak hilang saat browser tertutup tiba-tiba.
- **Ekspor data** — ekspor koleksi ke **Excel (.xlsx)** dan **PDF**.
- **Backup & restore** — cadangkan seluruh data ke file JSON dan pulihkan kapan saja.
- **Mode gelap/terang** — beralih tema dengan animasi transisi halus.
- **Kelopak sakura melayang** — efek visual ambient (otomatis nonaktif jika `prefers-reduced-motion` aktif).
- **Notifikasi toast** — umpan balik aksi (sukses/gagal/info) yang rapi dan tidak mengganggu.
- **Statistik koleksi** — ringkasan jumlah lagu, album, yang sudah didengarkan, dan favorit di bagian atas halaman.

## 🖥️ Teknologi

- **HTML, CSS, dan JavaScript murni** (vanilla) — tidak ada framework, tidak ada proses build.
- [`SheetJS (xlsx)`](https://cdnjs.cloudflare.com/ajax/libs/xlsx/) untuk ekspor Excel.
- [`jsPDF`](https://cdnjs.cloudflare.com/ajax/libs/jspdf/) + `jspdf-autotable` untuk ekspor PDF.
- Google Fonts: `Shippori Mincho`, `Zen Kaku Gothic New`, `JetBrains Mono`.
- Penyimpanan data menggunakan **`localStorage`** browser — 100% berjalan di sisi klien (client-side), tanpa server maupun database eksternal.

## 🚀 Cara Menjalankan

Tidak perlu instalasi atau dependensi apa pun.

1. Clone atau unduh repo ini:
   ```bash
   git clone https://github.com/<username>/sakura-melody.git
   ```
2. Buka file `sakura-melody.html` langsung di browser, **atau** jalankan lewat server lokal sederhana (disarankan agar semua fitur browser bekerja optimal):
   ```bash
   npx serve .
   # atau
   python3 -m http.server
   ```
3. Mulai tambahkan koleksi musikmu lewat tombol **+** di pojok kanan bawah.

## 💾 Tentang Data & Privasi

Seluruh data (daftar lagu, tag, genre custom, pengaturan tema, dll.) disimpan **secara lokal di browser** menggunakan `localStorage`. Artinya:

- Tidak ada data yang dikirim ke server mana pun.
- Data hanya tersedia di browser dan perangkat yang sama, kecuali diekspor secara manual.
- Gunakan fitur **Backup** secara berkala (menu Pengaturan) untuk menyimpan salinan data sebagai file JSON, terutama sebelum membersihkan cache browser atau berpindah perangkat.

## 📤 Ekspor & Impor

| Aksi | Format | Lokasi |
|---|---|---|
| Ekspor koleksi | `.xlsx` | Menu Pengaturan → Ekspor |
| Ekspor koleksi | `.pdf` | Menu Pengaturan → Ekspor |
| Backup penuh | `.json` | Menu Pengaturan → Backup |
| Restore data | `.json` | Menu Pengaturan → Restore |

## 🎨 Kustomisasi

Semua warna dan gaya diatur lewat **CSS custom properties** (`:root` dan `[data-theme="dark"]`) di bagian atas file, sehingga palet warna (sakura, matcha, emas, indigo, shu) bisa diubah dengan mudah tanpa menyentuh logika aplikasi.

## 📄 Lisensi

Proyek ini dirilis di bawah lisensi [MIT](LICENSE) — bebas digunakan, dimodifikasi, dan dibagikan.

---

<p align="center">🌸 Dibuat untuk mencatat lagu-lagu yang berkesan, satu kelopak sakura pada satu waktu.</p>
