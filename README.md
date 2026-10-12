# AuditGuard - Modul Voucher Kas Keluar
Dibuat oleh : Cantya Puspa/12030124140273

Aplikasi simulasi web untuk entri voucher transaksi kas keluar dan pemeriksaan jurnal auditor internal. Aplikasi ini dibuat sebagai antarmuka single-page HTML yang memungkinkan pengguna memasukkan data voucher, menyiapkan jurnal debit/kredit, memvalidasi keseimbangan saldo, dan menyimpan riwayat submit dalam sesi browser.

## Fitur Utama

- Entri header voucher:
  - No. Voucher
  - Tanggal transaksi
  - Nama penerima
  - Keterangan transaksi
- Entri detail jurnal akuntansi:
  - No. akun
  - Nama akun
  - Deskripsi baris
  - Nilai debit dan kredit
- Validasi otomatis:
  - Total debit harus sama dengan total kredit
  - Setiap baris harus memiliki akun dan nominal yang valid
  - Tombol submit aktif hanya jika data sudah memenuhi syarat
- Riwayat simulasi sesi:
  - Data voucher yang sudah disubmit tersimpan di memori browser
  - Bisa dilihat pada tabel arsip riwayat audit
- UI responsif dan modern:
  - Menggunakan Tailwind CSS
  - Desain sederhana untuk kebutuhan auditing internal

## Struktur File

- `web_app_utk_UTS.html` — berisi seluruh aplikasi web, layout, styling, dan logika JavaScript
- `README.md` — dokumentasi proyek

## Cara Menjalankan

Karena aplikasi ini berbasis HTML dan JavaScript murni, Anda dapat menjalankannya dengan salah satu cara berikut:

### 1. Buka langsung di browser
- Buka file `web_app_utk_UTS.html` di browser favorit Anda.
- Pastikan koneksi internet aktif karena aplikasi menggunakan CDN Tailwind CSS dan Font Awesome.

### 2. Jalankan local server (disarankan)

Pada folder proyek, jalankan command berikut:

```bash
python -m http.server 8000
```

Lalu buka alamat berikut di browser:

```text
http://localhost:8000/web_app_utk_UTS.html
```

## Deskripsi Aplikasi

Aplikasi ini mensimulasikan proses audit internal pada pengeluaran kas keluar. Pengguna dapat:

1. Mengisi nomor voucher dan data header
2. Menambahkan beberapa baris jurnal
3. Memilih akun dari daftar COA (Chart of Accounts)
4. Menentukan nominal debit dan kredit
5. Memastikan saldo seimbang sebelum submit
6. Menyimpan arsip voucher dalam riwayat sesi simulasi

## Catatan

- Data riwayat voucher disimpan hanya di memori browser saat sesi berjalan.
- Aplikasi ini merupakan versi simulasi dan belum terhubung ke database nyata.
- Nama proyek dan label UI mengacu pada kebutuhan modul pemeriksaan auditor internal dengan kemungkinan integrasi ke PostgreSQL / Supabase di masa depan.

## Teknologi yang Digunakan

- HTML5
- Tailwind CSS
- JavaScript vanilla
- Font Awesome Icons

## Lisensi

Proyek ini dibuat untuk keperluan tugas UTS / modul latihan audit internal dan dapat dimodifikasi sesuai kebutuhan pengembangan lebih lanjut.

