# Project 4 — Sistem Akademik (PHP OOP + Composer)

Aplikasi Sistem Akademik PHP OOP dengan autoload **Composer** (PSR-4: `App\` → `app/`).

## Fitur
- CRUD data mahasiswa
- Tampil data dosen dan matakuliah

## Struktur
- `composer.json` / `vendor/autoload.php` — autoload PSR-4
- `inc/Koneksi.php` — koneksi PDO
- `app/Mahasiswa.php` — model dalam namespace `App`
- `layouts/` — aset tampilan
- `database.sql` — skema `tb_mhsw`, `tb_dosen`, `tb_matakuliah`
- `index.php` — halaman utama + router `?hal=...`

## Instalasi
1. Letakkan folder ini di `htdocs` XAMPP.
2. Buat database `pbwl_samples_4`, lalu import `database.sql`.
3. Koneksi sudah diatur ke `127.0.0.1`, port **3307**, user `root`, password kosong, database `pbwl_samples_4`.
4. Buka `http://localhost/pbwl-samples-4/`.

Jika `vendor/` hilang, jalankan `composer install`.

## Catatan
File seperti `mhsw.php` adalah potongan view yang di-include lewat `index.php?hal=mhsw`, jadi bukan halaman mandiri.
