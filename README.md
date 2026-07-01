<div align="center">

# 📺 OrangeTV OS

### A custom Android TV firmware for Orange Pi 3B built through reverse engineering.

![Android](https://img.shields.io/badge/Android-11-green)
![Platform](https://img.shields.io/badge/Platform-RK3566-blue)
![Device](https://img.shields.io/badge/Device-Orange%20Pi%203B-orange)
![Status](https://img.shields.io/badge/Status-Development-yellow)
![License](https://img.shields.io/badge/License-Apache%202.0-lightgrey)

</div>

---

# About

OrangeTV OS is a custom Android TV operating system designed specifically for the Orange Pi 3B (RK3566).

Unlike traditional Android TV ports, this project is **built by understanding and recreating the Android TV environment through reverse engineering**.

The objective is to transform the stock Orange Pi Android firmware into a fully functional Android TV experience while maintaining compatibility with Rockchip firmware.

This project focuses on understanding how Android TV works internally instead of simply copying an existing ROM.

---

# Project Goals

- Build a native Android TV experience
- Maintain Rockchip compatibility
- Improve Google TV support
- Modernize bundled Google Apps
- Keep the firmware lightweight
- Document every modification
- Learn Android internals

---

# Current Features

- Android 11
- Dynamic Partitions
- Rebuilt super.img
- Updated Google Play Services
- Updated Play Store
- Updated SetupWizard
- Updated Leanback Launcher
- Updated Recommendations
- Updated SSS Auth Bridge
- TV Launcher
- TV Recommendations
- Root debugging support
- Custom system images

---

# Reverse Engineering Process

Instead of porting another ROM, this project studies the Android TV firmware and reproduces its behavior.

The workflow generally consists of:

```
Original Rockchip Firmware
            │
            ▼
 Firmware Extraction
            │
            ▼
 Reverse Engineering
            │
            ▼
 Android TV Analysis
            │
            ▼
 Google Apps Integration
            │
            ▼
 System Image Modification
            │
            ▼
 Dynamic Partition Rebuild
            │
            ▼
 Firmware Packaging
            │
            ▼
 Flash & Testing
```

---

# Development Workflow

1. Extract original firmware
2. Unpack Dynamic Partitions
3. Analyze Android TV framework
4. Reverse engineer Google TV components
5. Modify framework and system
6. Update Google Apps
7. Rebuild ext4 images
8. Generate new super.img
9. Package firmware
10. Flash to Orange Pi
11. Debug through ADB and Serial Console
12. Repeat

---

# Firmware Structure

```
super.img
├── system
├── vendor
├── product
├── system_ext
└── odm
```

---

# Tools Used

## Android Platform Tools

- adb
- fastboot

## Dynamic Partitions

- lpunpack
- lpmake
- lpdump
- simg2img
- img2simg

## Boot & Recovery

- magiskboot
- avbtool

## Rockchip

- afptool
- rkImageMaker
- rkdeveloptool

## Reverse Engineering

- apktool
- jadx
- aapt
- sqlite3

## Filesystem

- resize2fs
- e2fsck
- make_ext4fs
- losetup
- mount

## Linux Utilities

- file
- grep
- find
- sed
- du

---

# Google Components

Current integrated Google packages include:

- Google Play Services
- Google Play Store
- Google Services Framework
- Google Partner Setup
- Google Backup Transport
- Google One Time Initializer
- Google Ext Services
- SetupWraith
- Leanback Launcher
- TV Recommendations
- Katniss
- SSS Auth Bridge

---

# Current Issues

The project is still under active development.

Known issues include:

- Remote Service does not respond correctly from Google TV Remote on Android phones.
- Google TV setup process still requires additional compatibility improvements.
- Some Google TV components expect proprietary Google hardware.
- Further optimization of Google certification compatibility is required.
- Additional CTS compatibility improvements are planned.

---

# Roadmap

- [x] Dynamic Partitions
- [x] Working super.img rebuild
- [x] Updated GApps
- [x] Updated Play Store
- [x] Updated Play Services
- [x] Updated SetupWizard
- [x] Android TV Launcher
- [x] Google TV Components
- [ ] Remote Service Fix
- [ ] CTS Improvements
- [ ] Better Google TV Compatibility
- [ ] OTA Support
- [ ] Build Automation
- [ ] Documentation Expansion

---

# Supported Device

| Device | Status |
|---------|--------|
| Orange Pi 3B (RK3566) | Supported |

Future compatibility with other RK3566 devices is possible but not guaranteed.

---

# Philosophy

This project is primarily an educational effort focused on understanding Android TV internals.

Rather than porting an existing ROM, the goal is to rebuild the Android TV experience through careful analysis, reverse engineering, experimentation, and documentation.

Every successful modification helps improve the understanding of Android's framework, Google TV services, and the Rockchip platform.

---

# License

This repository only contains development work, scripts, patches and documentation.

Android, Google TV, Android TV and Google applications remain property of their respective owners.
