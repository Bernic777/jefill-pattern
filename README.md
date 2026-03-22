# Jefill Patterns Collection

Kumpulan pattern `awk` siap pakai untuk Jefill, khusus buat bantu ko pu kerja recon jadi lebih cepat, rapi, dan tra ribet. Ini cocok skali untuk anak-anak bug bounty yang biasa main filter URL, parameter, sampe cari celah-celah mantap dari hasil scan.

## Tentang Collection Ini

Di sini sa kumpul berbagai pattern yang sering dipake waktu hunting. Jadi ko tra usah pusing lagi tulis ulang `awk` panjang-panjang tiap kali kerja. Tinggal panggil nama pattern saja, langsung jalan.

Semua pattern di sini:
- Murni argumen `awk` saja (tra ada `awk`, tra ada pipe, tra ada chain command)
- Aman dipake (anti RCE, tra bisa disusupi script aneh-aneh)
- Siap langsung masuk ke Jefill tanpa modif banyak

## Cara Pake

1. Copy file pattern yang ko mau  
2. Taruh di folder:
   ~/.config/jefill/
3. Panggil pake Jefill:
   cat urls.txt | jefill namapattern

## Struktur Pattern

Setiap file dalam collection ini berisi satu pattern `awk`. Nama file jadi nama command waktu dipanggil di Jefill.

Contoh:
~/.config/jefill/xss.txt  
~/.config/jefill/lfi.txt  
~/.config/jefill/getjs.txt  

Panggil:
cat urls.txt | jefill xss

## Tujuan

Collection ini dibikin supaya:
- Hemat waktu waktu recon
- Kurangi kesalahan ketik command panjang
- Bikin workflow jadi lebih konsisten
- Tetap aman walaupun pakai pattern dari luar

## Catatan

Ko bebas tambah, ubah, atau sesuaikan pattern sesuai kebutuhan ko pu target. Kalo ada pattern baru yang lebih mantap, boleh dikumpul juga supaya makin lengkap.

Jalan pelan-pelan tapi pasti, yang penting hasil.
