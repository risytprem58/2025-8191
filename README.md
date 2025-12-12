Deskripsi
CVE-2025-8191 adalah kerentanan Cross-Site Scripting (XSS) pada Swagger UI yang digunakan di aplikasi macrozheng mall hingga versi 1.0.3.
Parameter configUrl pada /swagger-ui/index.html dapat dimanipulasi sehingga penyerang bisa menyisipkan skrip berbahaya.
Kerentanan ini bisa dieksploitasi dari jarak jauh, dan eksploitnya sudah dipublikasikan.

⚠️ Dampak
Penyerang dapat menjalankan JavaScript di browser korban.
Bisa mencuri cookie, token sesi, atau informasi sensitif lainnya.
Mengubah tampilan Swagger UI atau melakukan penipuan.
Pengguna bisa terkena serangan hanya dengan membuka URL Swagger UI yang sudah dimanipulasi.

🛡️ Rekomendasi
1. Perbarui Swagger UI ke versi terbaru (ganti folder swagger-ui lama).
2. Batasi akses Swagger UI, misalnya hanya untuk internal atau beri proteksi login.
3. Blokir parameter configUrl jika tidak digunakan untuk mencegah manipulasi.
