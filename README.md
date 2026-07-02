<p align="center">
  <img src="banner.png" alt="OrangeTV OS Banner" width="100%">
</p>

<h1 align="center">🍊 OrangeTV OS</h1>

<p align="center">
Custom Android TV firmware for Orange Pi 3B (RK3566), developed through reverse engineering.
</p>

<p align="center">

![Android](https://img.shields.io/badge/Android-11-3DDC84?style=for-the-badge&logo=android)
![Platform](https://img.shields.io/badge/RK3566-Orange%20Pi%203B-orange?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Development-yellow?style=for-the-badge)
![License](https://img.shields.io/badge/License-Apache%202.0-blue?style=for-the-badge)

</p>

---

# 📖 About

OrangeTV OS is an Android TV firmware created specifically for the **Orange Pi 3B (RK3566)**.

Unlike traditional ROM ports, this project is **not based on an existing Android TV ROM**.

Instead, the firmware is built by studying Google's Android TV implementation and recreating the required components through reverse engineering while adapting them to the Rockchip platform.

The goal is to provide a modern Android TV experience while keeping compatibility with Orange Pi hardware.

---

# ✨ Features

- Android 11
- Google TV / Android TV interface
- Dynamic Partitions support
- RK3566 optimized
- Google Play Services
- Google Play Store
- Leanback Launcher
- Google Assistant (Katniss)
- Recommendations support
- TV Provider
- OTA-ready structure
- Root-friendly

---

# 🏗 Development Philosophy

OrangeTV OS does **not** simply unpack an Android TV ROM and redistribute it.

Development includes:

- Reverse engineering Android TV firmware
- Framework adaptation
- Manual partition rebuilding
- Dynamic super image creation
- System image reconstruction
- Google application integration
- Compatibility fixes for Orange Pi hardware

---

# 🛠 Tools Used

During development the following tools are used:

- Android SDK Platform Tools
- adb
- fastboot
- afptool
- MagiskBoot
- simg2img
- img2simg
- lpmake
- lpdump
- lpadd
- avbtool
- MIO-KITCHEN
- SDDiskTool v1.72
- ext4 utilities
- Linux

---

# 📂 Repository Structure

```
OrangeTV
│
├── banner.png
│  
├── README.md
│
└── LICENSE
```

---

# 🚀 Flashing

The generated image can be written using:

- **SDDiskTool v1.72**

General process:

1. Download the latest release.
2. Extract the ZIP.
3. Open SDDiskTool.
4. Select the OrangeTV image.
5. Flash to a microSD.
6. Boot the Orange Pi 3B.

---

# 📦 Releases

Every release includes:

- OrangeTV image
- Release notes
- Installation instructions

---

# ⚠ Known Issues

Current issues being worked on:

- Google TV Remote Service does not respond correctly from the mobile app.
- Some Google TV components still require compatibility improvements.
- Additional device certification work is ongoing.
- Further optimization of Google Play integration.
- Hardware compatibility improvements.

---

# 🎯 Goals

- Stable Android TV experience
- Better hardware compatibility
- Google service compatibility
- OTA updates
- Improved performance
- Easier installation
- Open development

---

# 🤝 Contributing

Contributions are welcome.

Feel free to:

- Report bugs
- Suggest improvements
- Open Pull Requests
- Share testing results

---

# 📷 Screenshots

Screenshots will be added as development progresses.

---

# 📜 License

Apache License 2.0

---

# 👨‍💻 Author

**Erick Bernardo**

GitHub

https://github.com/ThisLaynOS

---

⭐ If you like this project, consider giving it a Star.
