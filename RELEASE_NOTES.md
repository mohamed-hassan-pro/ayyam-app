# Ayyam App — v1.0.0 Release Notes

## 🎉 Ayyam App — Initial Portfolio Release

**Version**: 1.0.0  
**Build Type**: Release APK (split per ABI)  
**Minimum Android Version**: Android 5.0 (API 21)  
**Target Android Version**: Android 14 (API 34)

---

## 📦 What's Included

This release includes three architecture-specific APKs optimized for different Android devices:

| APK File | Architecture | Target |
|---|---|---|
| `app-arm64-v8a-release.apk` | 64-bit ARM | Most modern Android phones (2017+) ✅ |
| `app-armeabi-v7a-release.apk` | 32-bit ARM | Older Android devices |
| `app-x86_64-release.apk` | x86 64-bit | Android emulators |

> **Recommended**: Download `app-arm64-v8a-release.apk` for most users.

---

## ✨ Features in This Release

- 🌙 **Islamic Event Tracker** — Tracks major Islamic events with accurate Hijri dates
- 📅 **Hijri Calendar** — Real-time Hijri ↔ Gregorian date conversion
- ⏳ **Countdown Timers** — Days remaining to each upcoming event
- 🔔 **Smart Notifications** — Local alerts configurable at 1 week, 1 month, 3 months, or 6 months before events
- 📖 **Rich Event Details** — Quran verses, hadiths, recommended practices per event
- 🌐 **Bilingual** — Full Arabic and English support with RTL layout
- 🎨 **Theming** — Dark / light / system mode with 10 card accent colors
- 💾 **Offline Support** — Events cached locally; works without internet after first load
- 🎓 **Interactive App Tour** — Guided walkthrough for new users
- 📲 **Onboarding Flow** — Profile setup with a smooth introduction experience

---

## 📥 Installation Instructions

1. Download the appropriate APK file for your device (see table above)
2. On your Android device, go to **Settings → Security** (or **Apps → Special Access**)
3. Enable **"Install from unknown sources"** (or "Install unknown apps" for your browser/file manager)
4. Open the downloaded APK file and tap **Install**
5. Launch **Ayyam** — complete the onboarding and enjoy!

---

## 🎬 Demo Video

The demo video (`ayyam_app_v1.mp4`) is attached to this release. Download it to see the app in action.

---

## 🔧 Build Info

```
Flutter: 3.x (stable channel)
Dart:    3.x
Build:   flutter build apk --split-per-abi
Signing: Debug keystore (portfolio release)
```

---

## 📝 Notes

- This is a **portfolio release** — the app is signed with a debug keystore
- Package ID: `com.example.ayyam_app`
- Internet required on first launch to fetch Islamic event dates from [Aladhan API](https://aladhan.com/islamic-calendar-api)
- Subsequent launches work offline (data cached with Hive)
