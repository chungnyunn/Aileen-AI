# Membuat APK Aileen hanya dengan HP

Proyek ini adalah prototipe awal, bukan aplikasi siap pakai. Untuk membangun APK tanpa laptop, gunakan GitHub Actions:

1. Ekstrak ZIP di HP (misalnya dengan Files/ZArchiver).
2. Buat repository baru di GitHub melalui browser, beri nama `AileenAndroid`.
3. Unggah isi folder `AileenAndroid` ke repository, termasuk folder tersembunyi `.github/workflows` dan file `build-apk.yml`.
4. Buka tab **Actions**, pilih **Build Aileen APK**, lalu tekan **Run workflow**.
5. Setelah proses selesai, buka hasil run dan unduh artifact **Aileen-debug-APK**. Ekstrak artifact ZIP untuk memperoleh `app-debug.apk`.
6. Buka APK di HP dan izinkan instalasi dari sumber yang digunakan, jika Android memintanya.

Catatan: workflow ini membangun APK debug dari source. Belum diuji pada Infinix Hot 9. Prototipe memakai Android SpeechRecognizer, bukan wake-word offline khusus. Deteksi panggilan saat layar mati tidak dijamin; Android/HiOS dapat membatasi mikrofon dan layanan latar belakang. Jalankan hanya ketika Aa Anan sengaja mengaktifkan layanan dan hentikan bila tidak digunakan.
