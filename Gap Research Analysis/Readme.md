# BAB II – GAP RESEARCH ANALYSIS

## 2.1 Status Quo: Kekuatan dan Kelemahan Pendekatan Eksisting

| Aspek | Penjelasan |
|-------|-------------|
| Kekuatan | Sistem deteksi kebocoran gas berbasis IoT dengan sensor MQ-2 dan mikrokontroler (ESP8266/ESP32) telah terbukti efektif dalam mendeteksi gas LPG secara real-time. Integrasi dengan Telegram Bot memungkinkan notifikasi cepat tanpa perlu sistem kompleks seperti server lokal. |
| Kelemahan | Sebagian besar penelitian hanya menampilkan hasil deteksi tanpa analisis kuantitatif terhadap kecepatan respon sistem dan akurasi pembacaan sensor dalam kondisi lingkungan yang bervariasi. |
| Celah Penelitian | Belum banyak penelitian yang menguji stabilitas sistem dan waktu respon notifikasi secara detail, serta membandingkan performa sistem dengan platform komunikasi lain seperti Blynk atau WhatsApp API. |

## 2.2 Research Gap (Celah Penelitian)

Beberapa penelitian relevan yang menjadi dasar pembentukan celah penelitian antara lain:

1. **Sari et al. (2022)**  
   Penelitian ini mengembangkan sistem deteksi kebocoran gas LPG menggunakan sensor MQ-2 yang dihubungkan dengan modul ESP8266. Sistem dapat mengirimkan notifikasi ke pengguna melalui Telegram Bot saat kadar gas melebihi ambang batas tertentu.  
   Namun, penelitian ini hanya menguji fungsionalitas dasar tanpa mengevaluasi kecepatan respon sistem, kestabilan koneksi Wi-Fi, serta tidak melakukan pengujian dalam kondisi lingkungan berbeda.

2. **Khahar et al. (2025)**  
   Penelitian ini mengimplementasikan IoT untuk sistem peringatan dini kebocoran gas yang terhubung dengan Telegram Bot. Mereka menambahkan tampilan monitoring sederhana berbasis web untuk menampilkan status sensor secara real-time.  
   Meski begitu, penelitian ini tidak membahas secara rinci performansi sistem dari sisi waktu kirim notifikasi, delay jaringan, serta ketahanan sistem saat koneksi internet tidak stabil.

3. **Apriliana et al. (2025)**  
   Penelitian ini berfokus pada analisis performa sensor MQ-2 dan ESP8266 dalam mendeteksi kebocoran gas. Mereka melakukan pengujian akurasi pembacaan sensor terhadap berbagai konsentrasi gas.  
   Walaupun memberikan analisis teknis sensor, penelitian ini tidak membahas integrasi sistem dengan platform notifikasi seperti Telegram maupun pengujian performa sistem secara end-to-end.

Dari ketiga penelitian tersebut dapat disimpulkan bahwa sebagian besar studi terdahulu berfokus pada pembangunan sistem deteksi dasar tanpa memperhatikan aspek **waktu respon, kestabilan komunikasi data, dan evaluasi sistem secara real-time di lingkungan nyata**.

Penelitian ini berupaya menutup kesenjangan tersebut dengan cara:

1. Mengukur akurasi sensor dan waktu respon sistem dari deteksi gas hingga pengiriman notifikasi ke Telegram.  
2. Melakukan pengujian pada kondisi jaringan yang berbeda untuk melihat kestabilan komunikasi data.  
3. Menghasilkan sistem IoT yang ekonomis dan aplikatif dengan antarmuka sederhana, mudah direplikasi oleh pengguna rumah tangga.

## 2.3 Novelty Penelitian

| Aspek | Kebaruan |
|-------|-----------|
| Metode | Pengembangan sistem pendeteksi kebocoran gas berbasis ESP8266/ESP32 dan sensor MQ-2 yang diintegrasikan dengan Telegram Bot API untuk notifikasi real-time. |
| Pendekatan | Penelitian tidak hanya membangun sistem, tetapi juga menganalisis waktu respon dan kestabilan sistem secara eksperimental. |
| Evaluasi | Menggunakan parameter evaluasi berupa akurasi deteksi, delay pengiriman notifikasi, serta stabilitas koneksi jaringan Wi-Fi. |
| Kontribusi Praktis | Memberikan solusi ekonomis, portabel, dan mudah diterapkan untuk sistem peringatan dini kebocoran gas LPG berbasis IoT di lingkungan rumah tangga. |

## Referensi

1. Sari, R., Pratama, Y., & Nugraha, D. (2022). Sistem Deteksi Kebocoran Gas LPG Menggunakan Sensor MQ-2 Berbasis Internet of Things (IoT). *Jurnal Teknik Informatika dan Komputer*, 8(1), 45–53.  
2. Khahar, F., Nurhayati, E., & Basuki, A. (2025). Implementasi IoT untuk Sistem Peringatan Dini Kebocoran Gas dengan Integrasi Telegram Bot. *Jurnal Elektronika dan Otomasi*, 6(2), 112–120.  
3. Apriliana, D., Setiawan, A., & Wibowo, R. (2025). Analisis Kinerja Sensor MQ-2 dan ESP8266 pada Sistem Deteksi Kebocoran Gas Real-Time. *Journal of Smart Devices and IoT Systems*, 4(1), 30–38.
