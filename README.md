# Communify
**Smart Transit Companion & Location-Based Audio Alert for Jabodetabek**

<p align="left">
  <img src="https://img.shields.io/badge/Platform-Android-000000?style=flat-square&logo=android&logoColor=white" alt="Platform" />
  <img src="https://img.shields.io/badge/Version-v1.0.0-24292e?style=flat-square" alt="Version" />
  <img src="https://img.shields.io/badge/Status-Public%20Beta-0969da?style=flat-square" alt="Status" />
  <img src="https://img.shields.io/badge/Coverage-Jabodetabek-1f2328?style=flat-square" alt="Coverage" />
</p>

[**Download APK (Latest Release)**](https://github.com/zyfdwm/communify-app/releases/latest) • [**Report an Issue**](https://github.com/zyfdwm/communify-app/issues) • [**Changelog**](#changelog)

---

### Overview

**Communify** is a lightweight, background-first transit assistant tailored for daily commuters across the Greater Jakarta (Jabodetabek) metropolitan area. Designed for hands-free navigation, Communify runs unobtrusively in the background to provide timely Indonesian voice prompts (Text-to-Speech) directly to your earphones or TWS, ensuring you never miss a transit interchange or your destination station.

---

### Key Capabilities

- **Automated Earphone Voice Alerts (TTS)**: Context-aware announcements for upcoming stations, transfer prep warnings, and arrival notifications without requiring you to check your screen.
- **Dual-Gate Geofencing (150m / 500m)**: Smart departure radius gating to eliminate false alarms while dwelling at departure platforms, paired with proactive 500m arrival zones.
- **Multi-Modal Routing Engine**: Shortest-path routing (Dijkstra) supporting multi-hop journeys with up-to-date platform switch instructions (Manggarai SO-7 layout, Tanah Abang new concourse).
- **Dead Reckoning Estimation**: Inertial estimation support during underground tunnels and dense signal-blocked segments.
- **Persistent Background Operation**: Runs as a prioritized Android Foreground Service with state persistence across app lifecycle events.
- **Offline Network Database**: Full local station and stop coordinate database—no active mobile data required for core geofence monitoring.
- **Route Simulator**: Built-in 1x–5x simulation engine with station jump controls for previewing routes before boarding.
- **Commute Carbon Analytics**: Automated travel logs with estimated CO₂ emission savings.

---

### Supported Transit Networks

Communify provides complete routing and coordinate mapping for 4 major regional systems:

```
[ Communify Transit Engine ]
├── KRL Commuter Line
│   ├── Bogor Line (Jakarta Kota - Bogor / Nambo)
│   ├── Cikarang Loop Line (Cikarang - Manggarai - Kampung Bandan)
│   ├── Rangkasbitung Line (Tanah Abang - Rangkasbitung)
│   ├── Tangerang & Tanjung Priok Lines
│   └── Soekarno-Hatta Airport Rail Link
├── Transjakarta BRT
│   ├── Corridors 1 - 14 (Full BRT Trunk Network)
│   └── Elevated Corridor 13 (Ciledug - Tendean)
├── MRT Jakarta
│   └── North-South Line (Lebak Bulus Grab - Bundaran HI Bank DKI)
└── LRT Network
    ├── LRT Jabodebek (Cibubur Line & Bekasi Line)
    └── LRT Jakarta (Pegangsaan Dua - Velodrome)
```

---

### Installation Guide (Android Sideload)

Because Communify is currently distributed directly via GitHub Releases:

1. **Download APK**: Download the latest release `.apk` file from the [Releases tab](https://github.com/zyfdwm/communify-app/releases/latest).
2. **Enable Unknown Sources**:
   - Open the downloaded file.
   - When prompted by Android security, navigate to **Settings** and toggle **"Allow from this source"** for your browser or file manager.
3. **Install & Launch**: Tap **Install**, then open Communify.
4. **Grant Permissions**:
   - **Location Permission**: Select **"Allow all the time"** (Background Location) so route tracking and earphone announcements remain active while your phone is locked or stored in your pocket.
   - **Notifications**: Allow notification access to enable heads-up status alerts.

---

### Changelog

#### v1.0.0 (Public Beta)
- Initial public beta release.
- Complete network coverage for KRL Commuter Line, Transjakarta Corridors 1–14, MRT Jakarta, and LRT Jabodebek/Jakarta.
- Indonesian TTS audio engine for background earphone guidance.
- Dijkstra transit routing with platform and interchange guidance.
- Dead reckoning tracking for tunnel segments.
- Built-in route simulation mode and commute carbon footprint tracker.

---

### Feedback & Contributing

To report routing discrepancies, missing bus stops, or suggest new features:
- File a report under [**GitHub Issues**](https://github.com/zyfdwm/communify-app/issues).
- Check the [**Discussions**](https://github.com/zyfdwm/communify-app/discussions) tab for community feature requests and roadmap updates.

---

<p align="left">
  <sub>Communify Transit Assistant • Jakarta Metropolitan Area</sub>
</p>
