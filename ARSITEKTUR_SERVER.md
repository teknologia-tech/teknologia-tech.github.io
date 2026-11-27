# Rencana backend (belum diimplementasikan)
Frontend statis ini tidak menerima data toko. Untuk layanan komersial gunakan hosting yang mengizinkan penggunaan komersial; GitHub Pages bukan server API. Pertahankan URL /privacy.html dan /delete-data.html saat migrasi atau gunakan redirect yang valid.

## Tahap 1
Backend HTTPS terpisah, verifikasi token pembelian dengan Google Play Developer API, validasi signature callback SSV AdMob dan transaksi unik (idempotensi), penyimpanan minimal hak akses. Jangan menerima klaim Premium dari client tanpa verifikasi. Tetapkan retensi, penghapusan, akses admin, audit dan rate limit; simpan secrets hanya di server. Source referensi memiliki PLAY_VERIFY_URL dan konfigurasi verifikasi Semi-Pro; audit kontrak aktual sebelum implementasi.

## Tahap 2 (opsional)
Autentikasi, isolasi tenant, backup cloud opt-in, sinkronisasi dengan konflik dan migrasi SQLite yang aman. Gunakan database terpisah, HTTPS, least privilege, pengujian pemulihan dan audit keamanan. Jangan memasukkan data pelanggan ke repository publik.

## AdMob
Tambahkan app-ads.txt di root domain hanya setelah menerima baris resmi dari AdMob. Daftarkan URL website di listing Play Store. Jangan menebak publisher ID.
