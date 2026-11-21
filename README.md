# Rantai Frasa

Game tebak rantai 6 kata (bahasa Indonesia) untuk beberapa kelompok. Tiap kelompok pegang satu HP, tanpa akun.

## Menjalankan
1. Aktifkan GitHub Pages: Settings > Pages > Source: "Deploy from a branch", pilih branch dan folder `/ (root)`.
2. Buka link Pages di semua HP.
3. Satu kelompok tekan "Buat room baru" (HP itu menjadi host), kelompok lain masukkan kode 4 huruf atau buka link yang disalin dari lobi.

## Catatan teknis
- Koneksi antar HP memakai PeerJS (WebRTC) lewat server perantara publik PeerJS. File `peerjs.min.js` (v1.5.4) disertakan di repo.
- Host menyimpan semua state dan kunci jawaban. HP lain hanya menerima kata yang sudah terbuka, jadi kunci tidak bisa diintip dari HP kelompok lain.
- Host harus tetap membuka halaman dan layar menyala. Kalau halaman host dimuat ulang, game dipulihkan dari penyimpanan lokal HP host.
- Jaringan yang membatasi koneksi (sebagian WiFi kantor/kampus) bisa menggagalkan sambungan. Cadangan: hotspot dari salah satu HP.
