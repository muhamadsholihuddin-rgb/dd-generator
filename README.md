# DD Generator

Generator **Laporan Kegiatan Pendamping Sosial — Program Keluarga Harapan** (format poster A2) untuk keperluan berkas sertifikasi pendamping sosial PKH.

Pengguna mengisi formulir (identitas, dasar hukum/SK, kegiatan, uraian 5 dimensi kompetensi TS/TMS/CMS/JRES/TRS, hasil), mengunggah foto dokumentasi, lalu mengunduh hasilnya sebagai **PDF** (ukuran kertas A2/A3/A4).

## Sifat & Privasi

- 100% statis, satu berkas `index.html` — tanpa backend, tanpa akun.
- Semua data diproses dan disimpan **di browser pengguna** (localStorage). Tidak ada data yang dikirim ke server.
- Logo resmi Kemensos & PKH tertanam di dalam berkas (base64).

## Cara Pakai

1. Buka halaman, isi formulir identitas dan kegiatan (bisa ditambah tanpa batas).
2. Unggah foto header dan foto dokumentasi tiap kegiatan; beri keterangan foto.
3. Klik **Unduh PDF** → pada dialog cetak pilih "Simpan sebagai PDF". Untuk ukuran persis A2 gunakan Chrome di komputer.
4. Tombol **Muat Contoh** menampilkan contoh isian lengkap.

## Deploy

- **GitHub:** unggah `index.html` dan `README.md` ke repo ini.
- **Vercel:** Import repo → framework "Other" → tanpa build command, output root. Setiap push ke `main` otomatis terbit (auto-deploy).

## Struktur Halaman PDF

1. Halaman 1 — kop & identitas, 01 Pendahuluan, 02 Dasar Hukum, daftar kegiatan.
2. Halaman per kegiatan — 03 Kegiatan yang Dilaksanakan (nama/waktu/tempat, pihak terlibat, uraian 5 dimensi, hasil, dokumentasi).
3. Halaman terakhir — 04 Penutup & tanda tangan, 05 Lampiran & galeri dokumentasi.
