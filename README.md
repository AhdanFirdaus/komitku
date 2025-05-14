# komitku 🚀

komitku adalah tools CLI sederhana berbasis Python yang membantu kamu membuat commit Git dengan format **Conventional Commit**, langsung dari terminal! Dibuat khusus untuk developer Indonesia, komitku menerjemahkan pesan commit dari bahasa Indonesia ke Inggris, memilih file untuk di-stage, dan memastikan proses commit jadi lebih cepat dan rapi. Tidak perlu bingung lagi dengan pesan commit yang berantakan! 😎

## Fitur Keren 🔥

- **Conventional Commit Otomatis**: Format pesan commit sesuai standar (misal, `feat(ui): add login button`).

- **Terjemahan Bahasa Indonesia**: Tulis pesan dalam bahasa Indonesia, komitku akan menerjemahkan ke Inggris.

- **Pilih File Interaktif**: Pilih file untuk di-stage dengan mudah, default ke semua file jika tekan Enter.

- **Scope Khusus untuk Config**: Tipe commit config otomatis tanpa scope tambahan.

- **Penanganan Ctrl+C**: Batalkan proses kapan saja tanpa meninggalkan file di staging area.

- **Tipe Commit Beragam**: Dukung berbagai tipe seperti `feat`, `fix`, `docs`, `config`, bahkan `wip` dan `sec`.

## Kenapa komitku? 🤔

Pernah lupa format commit yang benar? Atau bingung menerjemahkan pesan ke Inggris? komitku hadir sebagai teman setia yang:

- Membuat commitmu konsisten dan profesional.

- Menghemat waktu dengan otomatisasi.

- Ramah untuk developer Indonesia dengan input bahasa lokal.

## Instalasi 🛠️

1. **Pastikan Python 3.6+ terinstall**:
```sh
python --version
```

2. **Install dependensi**:
```sh
pip install deep-translator inquirer
```

3. **Clone repository ini**:
```sh
git clone https://github.com/AhdanFirdaus/komitku.git
cd komitku
```

4. **Jalankan tools**:
```sh
python commit_helper.py
```

## Cara Penggunaan 📖

1. **Jalankan di direktori Git**: Pastikan kamu berada di folder proyek yang sudah diinisialisasi dengan git init.
```sh
python commit_helper.py
```

2. **Pilih file untuk di-stage**:

- Gunakan panah dan spasi untuk memilih file.

- Tekan `Enter` untuk memilih semua file (default).

- Tekan `Ctrl+C` untuk membatalkan.

3. **Masukkan pesan commit**: Tulis pesan dalam bahasa Indonesia (misal, "Tambah fitur login").

4. **Masukkan scope (jika diperlukan)**:

- Untuk tipe `config` (misal, "Ubah konfigurasi"), scope otomatis kosong.

- Untuk tipe lain, masukkan scope seperti `ui`, `auth`, atau `api`.

5. **Konfirmasi**: Ketik `y` untuk commit atau `n` untuk batal.

6. **Selesai**! Cek hasilnya dengan:
```sh
git log --oneline
```
**Contoh**
```sh
=== Commit Helper ===

[Git Status]
Modified/Untracked: login.py

Pilih file untuk di-add (tekan Enter untuk All):
 [x] All (.)
 [ ] login.py
> (Enter)
Tidak ada file yang dipilih, menggunakan default: All
Berhasil git add semua file.

Masukkan pesan commit (bahasa Indonesia): Tambah fitur login
Pesan diterjemahkan: add login feature
Masukkan scope (contoh: ui, auth, api): auth
Pesan commit: ➕ feat(auth): add login feature
Konfirmasi commit? (y/n): y
[Success] Commit berhasil!
```

## Kontribusi 🤝

Ingin membuat komitku lebih keren? Fork repo ini, buat perubahan, dan kirim pull request!

## Lisensi 📜

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## Kontak 📬

Punya pertanyaan atau saran? Hubungi saya di GitHub atau buka issue di repo ini.

**komitku - Komit dengan gaya, ala Indonesia! 🇮🇩**