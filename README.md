# Communify Transit Assistant 🚆 🚌 🚇 🚊
> **Asisten Komuter Cerdas & Pengingat Stasiun/Halte Seluruh Moda Transportasi Jabodetabek**

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Android-3DDC84?style=for-the-badge&logo=android&logoColor=white" alt="Platform Android" />
  <img src="https://img.shields.io/badge/Version-v1.0.0-blue?style=for-the-badge" alt="Version" />
  <img src="https://img.shields.io/badge/Moda-KRL_%7C_TJ_14_Koridor_%7C_MRT_%7C_LRT-6366F1?style=for-the-badge" alt="Transport Networks" />
  <img src="https://img.shields.io/badge/Status-Public_Beta-2ea44f?style=for-the-badge" alt="Status" />
  <img src="https://img.shields.io/badge/License-Proprietary-red?style=for-the-badge" alt="License" />
</p>

<p align="center">
  <a href="https://github.com/zyfdwm/communify-app/releases/latest">
    <img src="https://img.shields.io/badge/📥_DOWNLOAD_APK-Versi_Terbaru_(v1.0.0)-2ea44f?style=for-the-badge&logo=android&logoColor=white" height="42" alt="Download APK" />
  </a>
</p>

---

## 📖 Apa itu Communify?

**Communify** adalah aplikasi asisten perjalanan *all-in-one* yang dirancang khusus untuk para pejuang komuter di wilayah metropolitan **Jabodetabek**. Pernahkah Anda ketiduran di KRL, asyik mendengarkan musik di bus Transjakarta hingga terlewat halte transit penting, atau kebingungan saat berpindah antarmoda di Kawasan Dukuh Atas dan Stasiun Manggarai?

Communify hadir sebagai solusi navigasi cerdas yang bekerja secara *hands-free* di saku Anda:
- 🎧 **Tetap Asyik Mendengarkan Musik/Podcast**: Suara asisten otomatis (*Text-to-Speech*) berbahasa Indonesia akan masuk ke earphone/TWS memberi tahu stasiun berikutnya, persiapan transit, hingga saat tiba di tujuan.
- 📍 **Pelacakan Latar Belakang (*Foreground Service*)**: Aplikasi tetap aktif mengawal perjalanan Anda saat layar HP mati atau terkunci di dalam saku celana/tas.
- 🔄 **Integrasi 4 Moda Transportasi Utama**: Menghubungkan seluruh jaringan rel dan bus BRT Jabodetabek dalam satu genggaman.

---

## 🚊 Cakupan Moda Transportasi Lengkap

Communify telah terintegrasi dengan database rute dan titik koordinat GPS presisi untuk 4 jaringan transportasi utama:

```
                  ┌─────────────────────────────────────────────────────────┐
                  │            COMMUNIFY TRANSIT ASSISTANT                  │
                  └──────┬─────────────┬─────────────┬─────────────┬────────┘
                         │             │             │             │
              ┌──────────┴──┐   ┌──────┴──────┐ ┌────┴──────┐ ┌────┴────────┐
              │ 🚆 KRL LINE │   │ 🚌 TJ BRT   │ │ 🚇 MRT JKT│ │ 🚊 LRT NET  │
              └─────────────┘   └─────────────┘ └───────────┘ └─────────────┘
               • Bogor Line      • 14 Koridor    • Lin Utara-  • LRT Jabodebek
               • Cikarang Loop     Utama BRT       Selatan       (Cibubur &
               • Rangkasbitung   • Rute Non-BRT    (Lebak Bulus   Bekasi Line)
               • Tangerang Line  • Koridor 13      s/d Bundaran• LRT Jakarta
               • Tanjung Priok     (Layang)        HI)           (Velodrome)
               • Bandara Soetta
```

### 1. 🚆 KRL Commuter Line
- **Lintas Bogor** (Jakarta Kota – Bogor / Nambo)
- **Lintas Cikarang Loop** (Cikarang / Bekasi – Jatinegara – Pasar Senen – Kampung Bandan – Manggarai)
- **Lintas Rangkasbitung** (Tanah Abang – Serpong – Parung Panjang – Rangkasbitung)
- **Lintas Tangerang & Tanjung Priok** (Duri – Tangerang & Jakarta Kota – Tanjung Priok)
- **Kereta Bandara Soekarno-Hatta (Basoetta)**

### 2. 🚌 Transjakarta BRT (14 Koridor Utama Penuh)
- **Koridor 1 s/d 14 Lengkap**: Mulai dari Koridor 1 (Blok M – Kota), Koridor 9 (Pinang Ranti – Pluit), Koridor 13 Jalur Layang Khusus (Ciledug – Tendean), hingga Koridor 14 (JIS – Senen Raya).
- Mendukung integrasi halte transfer sibuk (Harmoni Baru, Monas, Tosari, Semanggi, dll).

### 3. 🚇 MRT Jakarta
- **Lin Utara – Selatan**: Menghubungkan 13 stasiun bawah tanah dan layang dari Lebak Bulus Grab hingga Bundaran HI Bank DKI.

### 4. 🚊 LRT Network (Jabodebek & Jakarta)
- **LRT Jabodebek**: Lin Cibubur (Dukuh Atas – Harjamukti) & Lin Bekasi (Dukuh Atas – Jatimulya).
- **LRT Jakarta**: Lin Pegangsaan Dua – Velodrome Rawamangun.

---

## ✨ Fitur-Fitur Utama

| Fitur | Deskripsi |
| :--- | :--- |
| 🎧 **Voice Announcement (TTS Earphone)** | Notifikasi suara berbahasa Indonesia yang otomatis mengingatkan: *"Stasiun berikutnya...", "Bersiap turun/transit di...",* dan *"Anda telah tiba di stasiun tujuan"*. |
| 🔔 **Heads-Up Banner & Haptic Vibration** | Pop-up notifikasi berprioritas tinggi dan getaran haptik khusus saat kereta/bus memasuki radius 500m dari stasiun tujuan. |
| 🛡️ **Departure Radius Gate (150m)** | Algoritma cerdas yang mencegah alarm berbunyi berulang kali saat armada masih berhenti di peron stasiun keberangkatan. |
| 🗺️ **Routing & Transit Interchange Guide** | Pencarian rute tercepat (*Dijkstra Multi-Hop*) lengkap dengan panduan peron & pintu transit (Pola SO-7 Manggarai & JPO Integrasi Hub Dukuh Atas/CSW). |
| 🚇 **Dead Reckoning Estimation** | Estimasi pergerakan inersial cerdas saat armada melewati terowongan bawah tanah atau titik blank-spot GPS. |
| 🔋 **Hemat Kuota & Baterai** | Database halte/stasiun tersimpan secara *offline* di perangkat, tidak memerlukan koneksi internet aktif untuk geofencing. |
| 🌿 **Eco Impact Tracker** | Mencatat riwayat perjalanan Anda dan mengkalkulasi kontribusi penghematan jejak karbon (CO₂ Saved). |
| 🧪 **Mode Simulasi Virtual** | Ingin melihat simulasi rute sebelum berangkat? Uji rute perjalanan dengan kecepatan simulasi 1x–5x dan fitur *Lompat Stasiun*. |

---

## 📲 Panduan Instalasi APK di Android (Sideload)

Aplikasi Communify didistribusikan secara independen melalui GitHub Releases. Ikuti 4 langkah mudah berikut untuk menginstalnya:

```
  1. Unduh APK       2. Izinkan Sumber       3. Pasang APK        4. Izin Lokasi
 ┌──────────────┐    ┌──────────────┐       ┌──────────────┐     ┌──────────────┐
 │  Download    │───>│ "Allow from  │──────>│ Tekan Tombol │────>│ Izinkan GPS  │
 │  file .apk   │    │ this source" │       │  "Install"   │     │ "All the time│
 └──────────────┘    └──────────────┘       └──────────────┘     └──────────────┘
```

1. **Unduh File APK**:
   - Klik tombol [**Download APK Versi Terbaru**](https://github.com/zyfdwm/communify-app/releases/latest) atau unduh file `.apk` pada daftar *Assets*.
2. **Izinkan Instalasi dari Sumber Tidak Dikenal**:
   - Buka file `.apk` yang baru saja diunduh.
   - Jika muncul dialog keamanan Android, klik **Settings / Pengaturan** $\rightarrow$ centang **"Allow from this source / Izinkan dari sumber ini"** untuk browser atau file manager Anda.
3. **Pasang (Install) Aplikasi**:
   - Klik **Install / Pasang** dan tunggu proses selesai.
4. **Berikan Izin Lokasi (*Location Permission*)**:
   - Saat pertama kali membuka aplikasi, pilih **"Allow all the time / Izinkan sepanjang waktu"** untuk akses lokasi agar pengingat suara tetap dapat berbunyi saat layar HP mati atau di saku.

---

## 📝 Catatan Rilis & Blog Pembaruan (Changelog)

### 🚀 [v1.0.0] - Peluncuran Resmi Public Beta
*🗓️ Agustus 2026*
- 🚆 **Integrasi Multi-Moda Penuh**: Dukungan komprehensif untuk KRL Commuter Line, 14 Koridor Transjakarta BRT, MRT Jakarta, dan LRT Jabodebek/Jakarta.
- 🎧 **Sistem Audio TTS Bahasa Indonesia**: Pengumuman otomatis ke TWS/Headset untuk stasiun berikutnya dan peringatan transit.
- 🗺️ **Transit Navigation Engine**: Panduan peron terintegrasi (Manggarai SO-7, Hub Dukuh Atas, Stasiun Baru Tanah Abang).
- 📍 **Smart Geofence & Departure Gate (150m)**: Pelacakan latar belakang presisi anti-false alarm.
- 🧪 **Fitur Simulasi Virtual**: Fitur testing rute virtual dengan kontrol kecepatan.
- 📊 **Riwayat & Eco-Impact**: Kalender riwayat perjalanan interaktif dan kalkulator reduksi karbon.

---

## 💬 Laporan Bug & Saran Fitur (Feedback)

Communify dibuat dari komuter, oleh komuter, untuk komuter! Jika Anda menemukan rute yang perlu disesuaikan, nama halte baru, atau memiliki ide fitur:
- 🐛 **Lapor Bug / Request Rute**: Buat tiket di [**GitHub Issues**](https://github.com/zyfdwm/communify-app/issues).
- ⭐ **Dukung Aplikasi**: Berikan bintang (*Star*) pada repository ini agar lebih banyak pejuang komuter Jabodetabek terbantu!

---

<p align="center">
  Dibuat dengan ❤️ untuk Komuter Jabodetabek • <b>Communify Transit Assistant</b>
</p>
