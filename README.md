# Module 10 - Broadcast Chat

### 2.1. Original code of broadcast chat

![img](images/1.png)

Dari hasil percobaan tersebut, terlihat jelas bahwa setiap pesan yang dikirimkan oleh satu client akan diterima terlebih dahulu oleh server, lalu server secara otomatis mendistribusikan ulang pesan itu ke semua client yang sedang terhubung, termasuk pengirim asli. Mekanisme ini bekerja karena server menyimpan daftar koneksi client yang aktif dan terus-menerus menunggu input dari salah satu client untuk kemudian menyiarkan kembali pesan tersebut ke seluruh klien yang terhubung.