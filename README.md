# C.O.R ID HUB — versi 3 file

## Isi ZIP
1. index.html — seluruh website (HTML + CSS + JavaScript)
2. schema.sql — database Supabase
3. README.md — panduan

## CARA PASANG

### A. Buat database
1. Buka Supabase dan buat project.
2. Buka SQL Editor.
3. Copy semua isi `schema.sql`.
4. Jalankan SQL tersebut.

### B. Buat akun pemilik
Supabase → Authentication → Users → Add user.
Buat email dan password untuk akun pemilik.

### C. Masukkan koneksi database
Supabase → Project Settings → API.
Salin Project URL dan anon/publishable key.

Buka `index.html`, cari:
SUPABASE_URL="PASTE_SUPABASE_URL";
SUPABASE_KEY="PASTE_SUPABASE_ANON_OR_PUBLISHABLE_KEY";

Ganti dengan data Supabase kamu.

JANGAN masukkan service_role key.

### D. Upload ke GitHub
Ekstrak ZIP lalu upload hanya:
- index.html
- schema.sql
- README.md

Ketiga file harus berada langsung di folder utama repository.

Setelah upload: Settings → Pages → Deploy from branch → main → / (root) → Save.

## CATATAN
ID tersimpan di Supabase, jadi ID tidak hilang ketika browser ditutup.
Pengunjung hanya dapat melihat dan menyalin ID aktif.
Pemilik dapat login, menambah, dan menghapus ID.
