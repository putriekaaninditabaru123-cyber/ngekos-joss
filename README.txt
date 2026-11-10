CARA MEMBUAT FILE APK NGEKOS JOSS (tanpa Android Studio)

Kamu cukup punya akun GitHub (gratis). APK dibuat otomatis oleh GitHub.

1. Buka github.com, login (atau daftar).
2. Klik tanda + di kanan atas, pilih "New repository". Beri nama, misalnya ngekos-joss.
   Pilih Public, lalu klik "Create repository".
3. Di halaman repository, klik "uploading an existing file" (atau Add file > Upload files).
4. Ekstrak zip ini dulu. Lalu seret SEMUA isi foldernya ke halaman GitHub:
   folder app, folder .github, build.gradle, settings.gradle, gradle.properties.
   Tunggu sampai semua file terunggah, lalu klik "Commit changes".
5. CADANGAN kalau folder .github tidak ikut terunggah (sering terjadi karena namanya diawali titik):
   klik Add file > Create new file. Di kolom nama ketik persis:
   .github/workflows/build-apk.yml
   Lalu buka file workflow-build-apk.yml.txt dari zip ini, salin seluruh isinya, tempel, dan klik Commit.
6. Buka tab "Actions". Tunggu proses "Build APK" selesai sampai ada tanda centang hijau
   (sekitar 3 sampai 8 menit). Kalau belum jalan, klik "Build APK" di kiri lalu "Run workflow".
7. Ambil APK-nya: di halaman utama repository, lihat kanan "Releases", klik versi terbaru,
   lalu unduh NgekosJoss.apk dari bagian Assets. Itu file .apk langsung, bukan zip.
8. Unggah NgekosJoss.apk ke MediaFire, atau kirim langsung ke HP.

MEMASANG DI HP
- Buka file NgekosJoss.apk di HP Android (versi 8.0 ke atas).
- Kalau diminta, izinkan pemasangan dari sumber tidak dikenal untuk aplikasi yang kamu pakai membuka file.
- Kalau muncul peringatan Play Protect, pilih "Tetap instal". Itu muncul karena aplikasi tidak dari Play Store.

CATATAN
- Aplikasi butuh internet untuk peta dan data jalan. Jarak yang sudah dihitung tersimpan di aplikasi.
- Kalau proses Build gagal (tanda silang merah), buka run yang gagal, salin tulisan error di bagian yang merah, dan kirim ke Claude.
