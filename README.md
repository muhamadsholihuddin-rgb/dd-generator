# DD Generator

Generator **Laporan Kegiatan Pendamping Sosial — Program Keluarga Harapan** (format A4, tata letak baku hitam-putih tanpa warna dekoratif) untuk keperluan berkas sertifikasi pendamping sosial PKH.

Pengguna mengisi formulir (identitas, dasar hukum/SK, kegiatan, uraian 5 dimensi kompetensi TS/TMS/CMS/JRES/TRS, hasil), mengunggah foto dokumentasi, lalu mengunduh hasilnya sebagai **PDF** ukuran A4.

## Sifat & Privasi

- 100% statis, satu berkas `index.html` — tanpa backend, tanpa akun.
- Semua data diproses dan disimpan **di browser pengguna** (localStorage). Tidak ada data yang dikirim ke server.
- Logo resmi Kemensos & PKH tertanam di dalam berkas (base64).

## Penyusun Narasi Uraian Kegiatan

Setiap kegiatan punya kotak **Bahan Mentah Narasi** (kegiatan inti, sasaran, perencanaan, hambatan, cara mengatasi, alat/teknologi). Dari bahan itu uraian 5 dimensi kompetensi (TS/TMS/CMS/JRES/TRS) dapat disusun otomatis dengan dua cara:

1. **Susun Narasi (Lokal)** — mesin pola kalimat di dalam aplikasi; gratis, offline, tanpa kunci apa pun.
2. **Susun dengan AI Gemini** — opsional. Pengguna memasukkan **API Key Gemini miliknya sendiri** pada bagian "AI Gemini". Kunci **tidak ada di dalam kode** aplikasi ini; kunci tersimpan hanya di browser perangkat pengguna dan dipakai langsung dari perangkatnya ke Google. Buat kunci gratis di https://aistudio.google.com/apikey

Hasil susunan (lokal maupun AI) selalu dapat disunting manual sebelum dicetak.

## Cara Pakai

1. Buka halaman, isi formulir identitas dan kegiatan (bisa ditambah tanpa batas).
2. Unggah foto header dan foto dokumentasi tiap kegiatan; beri keterangan foto.
3. Klik **Unduh PDF** → pada dialog cetak pilih "Simpan sebagai PDF" (ukuran A4).
4. Tombol **Muat Contoh** menampilkan contoh isian lengkap.

## Deploy

- **GitHub:** unggah `index.html` dan `README.md` ke repo ini.
- **Vercel:** Import repo → framework "Other" → tanpa build command, output root. Setiap push ke `main` otomatis terbit (auto-deploy).

## Struktur Halaman PDF

1. Halaman 1 — kop & identitas, 01 Pendahuluan, 02 Dasar Hukum, daftar kegiatan.
2. Halaman per kegiatan — 03 Kegiatan yang Dilaksanakan (nama/waktu/tempat, pihak terlibat, uraian 5 dimensi, hasil, dokumentasi).
3. Halaman terakhir — 04 Penutup & tanda tangan, 05 Lampiran & galeri dokumentasi.
