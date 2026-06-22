<div align="center">

# SpeedX Coach

**Live team telemetry for the SpeedX athlete-tracking mesh.**
Every athlete's optical heart rate, pace, splits, and running stats — one screen, no router.

[![Latest version](https://img.shields.io/github/v/release/olam-source/speedx-coach-updates?label=version&color=2ea44f&style=for-the-badge)](https://github.com/olam-source/speedx-coach-updates/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/olam-source/speedx-coach-updates/total?color=36c5f0&style=for-the-badge)](https://github.com/olam-source/speedx-coach-updates/releases)
![Platforms](https://img.shields.io/badge/macOS%20·%20Windows%20·%20Linux-8957e5?style=for-the-badge)

</div>

---

## Download

Pick your platform — no account needed.

| | Platform | Get it |
|:--:|:--|:--|
| 🍎 | **macOS** — Apple Silicon (M-chips) | **[Download&nbsp;.dmg&nbsp;»](https://github.com/olam-source/speedx-coach-updates/releases/download/v0.6.0/SpeedX-Coach-0.6.0-arm64.dmg)** |
| 🍎 | **macOS** — Intel | **[Download&nbsp;.dmg&nbsp;»](https://github.com/olam-source/speedx-coach-updates/releases/download/v0.6.0/SpeedX-Coach-0.6.0-x64.dmg)** |
| 🪟 | **Windows** 10 / 11 | **[Download&nbsp;.exe&nbsp;»](https://github.com/olam-source/speedx-coach-updates/releases/download/v0.6.0/SpeedX-Coach-0.6.0-x64.exe)** |
| 🐧 | **Linux** (x86-64) | **[Download&nbsp;.AppImage&nbsp;»](https://github.com/olam-source/speedx-coach-updates/releases/download/v0.6.0/SpeedX-Coach-0.6.0-x86_64.AppImage)** |

<sub>Newest build is always on the **[latest release »](https://github.com/olam-source/speedx-coach-updates/releases/latest)** page.</sub>

## Install

<details>
<summary><b>macOS</b></summary><br>

1. Open the `.dmg` and drag **SpeedX Coach** into **Applications**.
2. First launch only: **right-click the app → Open → Open** (one-time Gatekeeper step — the build isn't notarized yet).
</details>

<details>
<summary><b>Windows</b></summary><br>

Run the `.exe`. If SmartScreen appears: **More info → Run anyway** (unsigned build).
</details>

<details>
<summary><b>Linux</b></summary><br>

```bash
chmod +x SpeedX-Coach-*.AppImage
./SpeedX-Coach-*.AppImage
```
</details>

## What it does

Plug the SpeedX **coach hub** into your laptop via USB and every athlete's wearable appears live on one screen. Each wearable is a compact ESP32-S3 armband with a **MAXM86161 optical PPG sensor** for wrist heart rate — no chest strap needed. The wearables also broadcast a standard **BLE Heart Rate** signal so athletes can pair their Garmin, Coros, or Apple Watch at the same time.

**~$30/athlete in hardware. Full 15-athlete team kit: ~$450.**

- **Heart rate** — optical wrist HR with training-zone coloring (Z1–Z5)
- **Pace** per mile, current & best **split**, **distance**, cadence, stride, speed
- Link quality, battery level, GPS / lap / low-battery badges per athlete
- **Athlete roster** — map node IDs to real names and teams; saved between sessions
- **Team filtering** — filter the board to one team with a click
- **Per-athlete history charts** — live HR, pace, and distance charts; no external library
- **Session recording → CSV** export for post-session analysis
- **Low-battery & HR-zone alerts** shown in the header bar and on the card
- **First-run tutorial** — a 4-step guided overlay walks new coaches through the full workflow on first launch
- **In-app updates** — the app checks for new versions and downloads + opens the installer for you; no signing certificate required

## What's new in v0.6.0

- **In-app updates** — SpeedX Coach now updates itself. It checks the releases repo, downloads the right installer for your platform, and opens it (one drag on macOS). There's a **Check for updates** button in the rail, plus a quiet check on launch. *(The build you have installed needs one manual update to 0.6.0; every version after that updates in-app.)*
- **Single control-rail layout** — brand, Connect, session controls, and roster live in one elegant left rail; the main area is a clean board of live cards
- **"Atelier" look** — obsidian + champagne-gold + ivory palette with serif display type
- Reflows cleanly at any window size
- First-run coach tutorial; MAXM86161 optical PPG armband; BLE Heart Rate broadcast

---

<div align="center"><sub>This repository hosts the installers only. The application source lives in a private repository.</sub></div>
