# Jam Digital dengan LCD 20x4, RTC DS3231, dan Buzzer

Proyek ini adalah implementasi jam digital sederhana menggunakan Arduino Uno yang menampilkan waktu, tanggal, dan hari pada layar LCD 20x4. Modul RTC DS3231 digunakan untuk menjaga akurasi waktu, dan buzzer memberikan bunyi detik sebagai indikator.

## Fitur

- **Tampilan Waktu Real-Time**: Menampilkan jam, menit, dan detik dalam format 24 jam.
- **Tampilan Tanggal dan Hari**: Menunjukkan hari dalam bahasa Indonesia, tanggal, bulan, dan tahun.
- **Bunyi Detik**: Buzzer berbunyi setiap detik untuk indikasi waktu.
- **Pesan Tetap**: Menampilkan nama institusi di baris bawah LCD.

## Persyaratan Hardware

- Arduino Uno
- LCD 20x4 (dengan modul I2C atau pin langsung)
- Modul RTC DS3231
- Buzzer pasif
- Kabel jumper
- Breadboard (opsional)

## Persyaratan Software

- PlatformIO IDE
- Arduino Framework
- Library:
  - LiquidCrystal (fmalpartida/LiquidCrystal@^1.5.0)
  - RTClib (adafruit/RTClib@^2.1.4)

## Instalasi

1. **Clone Repository**:
   ```
   git clone <url-repo-ini>
   ```

2. **Buka di PlatformIO**:
   - Buka PlatformIO IDE.
   - Buka folder proyek ini.

3. **Install Dependencies**:
   - PlatformIO akan otomatis mengunduh library yang diperlukan berdasarkan `platformio.ini`.

4. **Build dan Upload**:
   - Sambungkan Arduino Uno ke komputer.
   - Klik tombol Build dan Upload di PlatformIO.

## Penggunaan

1. **Persiapan Hardware**:
   - Sambungkan LCD, RTC DS3231, dan buzzer ke Arduino sesuai dengan pin yang didefinisikan dalam kode (`main.cpp`).
   - Lihat `diagram.json` atau simulasi Wokwi untuk diagram rangkaian.

2. **Jalankan Program**:
   - Setelah upload, Arduino akan menampilkan judul proyek selama 1 detik, kemudian mulai menampilkan waktu.
   - RTC akan disetel ke waktu kompilasi jika kehilangan daya.

3. **Simulasi**:
   - Gunakan `wokwi.toml` untuk mensimulasikan proyek di platform Wokwi.

## Diagram Rangkaian

Diagram rangkaian tersedia dalam file `diagram.json`. Anda dapat mengimpornya ke Wokwi atau alat simulasi lainnya untuk melihat koneksi hardware.

## Struktur Proyek

```
├── diagram.json          # Diagram rangkaian
├── platformio.ini        # Konfigurasi PlatformIO
├── wokwi.toml            # Konfigurasi simulasi Wokwi
├── include/              # Header files
├── lib/                  # Library dependencies
├── src/
│   └── main.cpp          # Kode utama Arduino
└── test/                 # Test files
```

## Lisensi

Proyek ini dibuat untuk tujuan edukasi. Silakan gunakan dan modifikasi sesuai kebutuhan.

## Kontribusi

Jika Anda ingin berkontribusi, silakan buat pull request atau laporkan issue.

## Kontak

Untuk pertanyaan, hubungi [nama/email Anda].