# 🚀 Guru Mitra

> *Just‑in‑time classroom coach — APK demo (WhatsApp bot + mobile app)*

<p align="center">
  <a href="https://github.com/<your-org>/gurumitra/releases/latest" target="_blank" rel="noopener">
    <img src="https://img.shields.io/badge/Download%20APK-%E2%86%93-brightgreen" alt="Download APK" />
  </a>
  &nbsp;&nbsp;
  <a href="https://github.com/<your-org>/gurumitra/blob/main/LICENSE" target="_blank">
    <img src="https://img.shields.io/badge/License-MIT-green.svg" alt="License" />
  </a>
  &nbsp;&nbsp;
  <img src="https://img.shields.io/badge/Status-Demo%20Ready-blue.svg" alt="Status" />
</p>

---

## 🎯 Quick Summary

**Guru Mitra** is a voice-first assistant that helps primary‑school teachers solve live classroom problems via WhatsApp and a lightweight Android app (APK). Teachers send a short voice note and receive short, actionable fixes (2–4 steps), a teacher script (15–30s), and translation/TTS playback — all optimized for low-bandwidth, multi‑grade contexts.

---

## ✨ Features

* ✅ **Voice-first**: Speak your problem in-app or on WhatsApp.
* ✅ **Voice & Text replies**: Teacher-ready voice notes and short text steps.
* ✅ **Localized**: Translation + TTS support for local languages.
* ✅ **Offline-friendly**: Cached templates for low connectivity.
* ✅ **Fast**: Designed for 15–60s interaction round-trips.

---

## 🖼 Demo Media

> Add your images and videos to `/assets/media/` and attach the APK in Releases. Replace placeholders with real file names.

**Screenshots**

|                                WhatsApp Bot (1) |              Mobile App (3)              |
| ----------------------------------------------: | :--------------------------------------: |
| ![WhatsApp Bot](/assets/media/whatsappPhoto.jpg) | ![App 1](/assets/media/appPhoto1.jpg) |
|                                                 | ![App 2](/assets/media/appPhoto2.jpg) |
|                                                 | ![App 3](/assets/media/appPhoto3.jpg) |

## 🎥 Watch the Demos

<div align="center">

[![App Demo](https://img.youtube.com/vi/YOUR_APP_VIDEO_ID/maxresdefault.jpg)](https://youtu.be/YOUR_APP_VIDEO_ID)
**App walkthrough** • 30–60s • _TTS, quick fixes_

&nbsp;&nbsp;&nbsp;

[![WhatsApp Demo](https://img.youtube.com/vi/YOUR_WA_VIDEO_ID/maxresdefault.jpg)](https://youtu.be/YOUR_WA_VIDEO_ID)
**WhatsApp bot demo** • 30–60s • _Voice note → reply_

</div>


> Tip: For GitHub Releases, attach the APK and video files. Large media can be attached to the Release or hosted externally (YouTube/Vimeo) and linked here.

---

## 🧭 How the demo works (one‑liner flow)

`Teacher (voice) → WhatsApp / App → Audio conversion (ffmpeg) → LLM (prompt + teacher context) → TTS → WhatsApp voice note / In‑app playback`

---

## 🧩 Tech Stack (icons)

<p>
  <img alt="Flutter" src="https://img.shields.io/badge/Flutter-02569B?logo=flutter&logoColor=white" />
  <img alt="Node.js" src="https://img.shields.io/badge/Node.js-43853D?logo=node.js&logoColor=white" />
  <img alt="Baileys" src="https://img.shields.io/badge/Baileys-FFCB2E?logo=whatsapp&logoColor=white" />
  <img alt="FFmpeg" src="https://img.shields.io/badge/FFmpeg-202020?logo=ffmpeg&logoColor=white" />
  <img alt="OpenAI/Gemini" src="https://img.shields.io/badge/LLM-Gemini-4B8BF5?logo=openai&logoColor=white" />
  <img alt="Hive" src="https://img.shields.io/badge/Hive-FFCA28?logo=hive&logoColor=black" />
</p>

---

## ⚙️ Included in this Release

* `app-release.apk` — universal APK (attach to Releases)
* Demo screenshots (placeholders under `/assets/media/`)
* Short demo videos (app + WhatsApp)

> **Note:** Source code is not included in this repo release. This is a demo-only release for distribution and judging.

---

## 📥 Download & Install

1. Go to the **Releases** page and download `app-release.apk`.
2. Install on Android device: `adb install app-release.apk` or open the APK on your phone.

---

## 🛡 Security & Privacy Notes

* Do **not** hardcode API keys in the APK. Use server-side tokens for production.
* Keep teacher data private: anonymize PII in analytics.

---

## 🧭 Run the demo locally (for maintainers)

* Attach demo media under `/assets/media/`.
* Add `app-release.apk` as a Release asset.
* Update links in this README.

---

## 🧾 License

MIT — see `LICENSE`.

---

## 👥 Team

* **Krishna Sharma** — [krishnasharma.active@gmail.com](mailto:krishnasharma.active@gmail.com) — 7906839138
* **Mukul Sharma** — [mukulpanditkana@gmail.com](mailto:mukulpanditkana@gmail.com) — 6397722693

---

## 🎬 Want help preparing release assets?

I can:

* generate optimized screenshot templates (phone frames),
* create a short demo GIF from your video, or
* produce a polished Release description for GitHub.


