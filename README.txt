NEXTY MINE — GITHUB PAGES

Akun GitHub: nextystudio1
Nama repository yang disarankan: nexty-mine
Alamat situs setelah GitHub Pages aktif:
https://nextystudio1.github.io/nexty-mine/

LANGKAH 1 — BUAT REPOSITORY
1. Masuk ke https://github.com/new
2. Repository name: nexty-mine
3. Pilih Public agar GitHub Pages gratis dapat digunakan.
4. Klik Create repository.
5. Upload index.html dan README.txt dari ZIP ini ke root repository, lalu Commit changes.

LANGKAH 2 — AKTIFKAN GITHUB PAGES
1. Buka repository nexty-mine.
2. Masuk Settings → Pages.
3. Pada Build and deployment, pilih Deploy from a branch.
4. Branch: main; folder: / (root). Klik Save.
5. Tunggu sampai URL Pages tampil aktif.

LANGKAH 3 — ATUR SUPABASE AUTH
Buka Supabase project → Authentication → URL Configuration.
Site URL:
https://nextystudio1.github.io/nexty-mine/

Tambahkan URL yang sama pada Redirect URLs (Additional Redirect URLs), lalu Save.

PENTING
- Jangan gunakan alamat file:///C:/... atau localhost.
- Jika nama repository diubah, URL GitHub Pages dan URL Supabase harus ikut disesuaikan.
- Pendaftaran sudah mengirim emailRedirectTo ke folder situs yang sedang dibuka.
- Kunci anon/publishable di frontend memang boleh dipakai bersama RLS; jangan pernah menaruh service_role/secret key di index.html.
- Setelah hosting aktif, uji daftar akun baru dan pastikan tautan email kembali ke URL GitHub Pages.
