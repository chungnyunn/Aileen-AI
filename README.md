# Aileen — starter Android project

Proyek awal Android Studio untuk Infinix Hot 9 / Android. Fitur prototipe:
- meminta izin overlay dan menampilkan gambar karakter Aileen sebagai jendela mengambang;
- layanan suara foreground dengan notifikasi yang terlihat;
- percobaan deteksi kata "Aileen" memakai Android SpeechRecognizer bahasa Indonesia;
- balasan suara memakai TextToSpeech sistem (kualitas/suara tergantung mesin TTS yang terpasang).

## Cara membuka dan mencoba
1. Buka folder ini di Android Studio pada komputer.
2. Tunggu Gradle Sync dan pasang Android SDK 35 jika diminta.
3. Hubungkan Infinix Hot 9 dengan USB debugging, lalu Run aplikasi.
4. Izinkan mikrofon dan "Tampilkan di atas aplikasi lain".
5. Tekan **Mulai dengarkan 'Aileen'**. Notifikasi permanen menandakan layanan mikrofon aktif.
6. Ucapkan "Aileen" untuk mencoba memunculkan karakter.

## Batasan penting
Ini adalah source project prototipe, bukan APK siap instal. Lingkungan pembuatan ini tidak memiliki Android SDK/Gradle untuk membangun dan menguji APK. SpeechRecognizer Android bukan mesin wake-word selalu aktif: pengenalan dapat berhenti, memerlukan internet/layanan Google, atau dibatasi oleh sistem/penghemat baterai Infinix. Tidak dijamin mendengar saat layar mati. Jangan gunakan untuk percakapan sensitif; mikrofon aktif selama layanan berjalan. Hentikan lewat tombol di aplikasi.

Untuk versi produksi perlu implementasi wake-word offline khusus, penanganan lifecycle audio yang benar, animasi karakter Live2D, pengujian perangkat, dan build/sign APK.
