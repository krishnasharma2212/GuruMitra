# Guru Mitra

**Just‑in‑time classroom coach — WhatsApp bot + lightweight Flutter app**

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE) [![Status](https://img.shields.io/badge/status-demo%20ready-blue.svg)](#)

---

<p align="center">
  <!-- Replace the link below with your real hosted APK link or GitHub release asset -->
  <a href="https://example.com/app-release.apk" target="_blank" rel="noopener">
    <img src="https://img.shields.io/badge/Download%20APK-%E2%86%93-brightgreen" alt="Download APK" />
  </a>
</p>

---

## What is Guru Mitra?

Guru Mitra is a voice-first assistant for primary‑school teachers. It delivers quick, classroom-ready fixes (2–4 steps), a short teacher script, and management tips — delivered via WhatsApp voice notes or a lightweight mobile app. Designed for low-bandwidth, multi‑grade, and rural contexts.

## Highlights

* Voice input & voice output (WhatsApp + app)
* Short actionable micro-interventions (15–30s teacher scripts)
* Localized & translation-ready responses
* Offline-first app with cached templates for low connectivity
* CRP dashboard-ready: aggregate queries for mentors

---

## Screenshots

> Replace the image paths with your actual screenshot files in `/assets/screenshots/`.

**WhatsApp bot (1):**

![WhatsApp Bot Screenshot](/assets/screenshots/whatsapp_bot.png)

**Mobile App (3):**

![App Screenshot 1](/assets/screenshots/app_screen_1.png)
![App Screenshot 2](/assets/screenshots/app_screen_2.png)
![App Screenshot 3](/assets/screenshots/app_screen_3.png)

---

## Quick Demo (what you’ll see)

1. Teacher records a short voice note in-app or on WhatsApp.
2. Bot forwards audio to the LLM orchestrator.
3. Model returns 2–4 actionable steps + a 15–30s teacher script.
4. Bot converts response to a WhatsApp-compatible voice note and sends it back.
5. Teacher hears or reads the reply, applies the fix, and optionally rates it.

---

## Download APK

Click the badge above or use this link (replace with actual asset):

**Download:** [app-release.apk](https://example.com/app-release.apk)

*To attach the real APK to your repo:* push the APK to the GitHub Releases page and replace the link above with the release asset URL.

---

## Getting started (Developer)

> The repo contains two main parts: `bot/` (Node.js + Baileys) and `app/` (Flutter).

### Prerequisites

* Node.js 18+ and npm/yarn
* Java JDK 11+, Android SDK
* Flutter SDK (stable) + Android toolchain
* ffmpeg installed on the server for audio conversion

### Bot (quick start)

```bash
cd bot
cp .env.example .env
# Put your secrets into .env (do NOT commit real keys)
npm install
node engine.js
```

**Important:** Never commit your real API keys. Use environment variables and revoke any keys accidentally exposed.

### App (quick start)

```bash
cd app
flutter pub get
flutter run --release
# or build a single universal APK
flutter build apk --release
```

---

## Architecture (short)

```
Teacher (WhatsApp / Flutter app) 
  -> WhatsApp Bot (Baileys) or App endpoint
  -> Audio conversion (ffmpeg) -> LLM Orchestrator (prompts + context)
  -> TTS -> Format as WhatsApp voice note -> Delivered back to teacher
  -> Feedback stored for analytics & CRP dashboard
```

---

## Configuration notes

* Replace hard-coded keys with environment variables (`OPENAI_API_KEY`, `WHATSAPP_AUTH`, etc.).
* Keep `debug-info` from obfuscation in a secure place (if you use `--obfuscate`).
* Use Play App Signing for production distribution.

---

## Contributing

Contributions are welcome! Please open an issue or PR. Suggested areas:

* Improve prompt templates for better pedagogy
* Add language packs (Hindi/Hinglish) and localization
* CRP dashboard visualizations

---

## Team

* **Krishna Sharma** — [krishnasharma.active@gmail.com](mailto:krishnasharma.active@gmail.com) — 7906839138
* **Mukul Sharma** — [mukulpanditkana@gmail.com](mailto:mukulpanditkana@gmail.com) — 6397722693

---

## License

This project is released under the **MIT License**. See `LICENSE` for details.

---

## Contact

Questions? Email Krishna Sharma at `krishnasharma.active@gmail.com`.

---

*Replace placeholder links and image paths with real assets before publishi
