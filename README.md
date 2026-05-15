# 🌀 Smart Greenhouse Fan (Cooling System)

Sistem pendinginan otomatis untuk Greenhouse menggunakan Kipas DC yang dikendalikan berdasarkan suhu aktual melalui Blynk IoT Cloud.

## 🚀 Fitur
- **🌐 Dual-Mode**: Hardware (WiFiManager) & Simulation (Wokwi).
- **📊 Monitoring**: Suhu, Kelembapan Udara, & Tanah via Blynk.
- **🛡️ Fail-Safe**: Pengaman pompa air (Max 15s).
- **🌀 Auto-Cooling**: Kipas menyala otomatis jika suhu > 30°C.

## 🛠️ Persiapan
1. Install ekstensi **PlatformIO** & **Wokwi** di VSCode.
2. Edit `src/main.cpp` & `src/main_sim.cpp` untuk memasukkan Blynk Auth Token Anda.

## 📤 Upload & Simulasi
Panduan konfigurasi lingkungan (Environment) dapat dilihat pada file `platformio.ini`. Gunakan environment `hardware` untuk perangkat fisik atau `simulation` untuk pengujian via Wokwi.

## 🗺️ Pin Mapping
- DHT22: `GPIO 16`
- Soil Moisture: `GPIO 35`
- Relay Pompa: `GPIO 5`
- Relay Kipas: `GPIO 18`
- LCD: `I2C (21, 22)`

---
Detail teknis lebih lanjut silakan baca [PENJELASAN.md](./PENJELASAN.md).
