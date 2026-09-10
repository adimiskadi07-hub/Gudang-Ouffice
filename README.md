Panduan Deployment GitHub Pages & Google Sheets Synchronization

Aplikasi Ouffice.co.id - Sistem Inventaris Gudang dapat dijalankan langsung di GitHub Pages (atau Vercel / Netlify / Domain sendiri) dan tersinkronisasi 100% secara live real-time dengan Google Sheets Anda.

🚀 LANGKAH 1: Setup Google Sheets Backend (Apps Script)

Buka Google Sheets dan buat Spreadsheet baru bernama "Database Inventaris Gudang".

Klik menu Ekstensi > Apps Script.

Hapus seluruh isi file Code.gs lama, lalu tempelkan seluruh isi file Code.gs dari repository ini.

Simpan file (Ctrl + S).

Di sudut kanan atas Apps Script Editor, klik Deploy (Terapkan) > New deployment (Penerapan baru).

Klik ikon gerigi ⚙️ > Pilih Web app (Aplikasi Web).

Konfigurasikan:

Execute as (Jalankan sebagai): Me (Saya / Email Anda)

Who has access (Siapa saja yang memiliki akses): Anyone (Siapa Saja)

Klik Deploy. Berikan otorisasi izin jika diminta oleh Google.

Salin Web App Executable URL yang dihasilkan (contoh: https://script.google.com/macros/s/AKfycb.../exec).

📦 LANGKAH 2: Setup Repository di GitHub

Buat repository baru di GitHub (misalnya: ouffice-inventaris-gudang).

Unggah file Index.html dan README.md ke repository GitHub tersebut.

Buka tab Settings di repository GitHub Anda.

Pilih menu Pages di panel sebelah kiri.

Pada bagian Build and deployment > Branch, pilih branch main (atau master) dan folder / (root), lalu klik Save.

GitHub akan memublikasikan website Anda di URL: https://<username>.github.io/<repository-name>/.

🔗 LANGKAH 3: Hubungkan GitHub Pages dengan Google Sheets

Buka URL website GitHub Pages Anda (atau jalankan file Index.html di browser Anda).

Klik badge tombol 🟢 Atur URL Google Sheets atau ikon Gerigi (⚙️) di pojok kanan atas header aplikasi.

Tempelkan URL Web App Google Apps Script dari Langkah 1.

Klik Simpan & Hubungkan.

Aplikasi kini sepenuhnya aktif dalam Mode Siap Pakai Live, dan seluruh transaksi tambah, edit, hapus, serta scan QR code akan langsung tersimpan secara otomatis ke Google Sheets Anda secara real-time.
