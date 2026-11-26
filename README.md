# EQify

**An Android equalizer that follows your music.** EQify switches tone by genre on its own while you listen, and corrects your exact headphones with AutoEQ profiles.

> **Beta.** EQify is in public beta. Expect rough edges, and please [report anything odd](../../issues/new/choose).

<!-- Add screenshots to a screenshots/ folder and uncomment:
<p>
  <img src="screenshots/home.png" width="200">
  <img src="screenshots/eq.png" width="200">
  <img src="screenshots/headphones.png" width="200">
</p>
-->

## Features

- **Automatic genre EQ.** It detects the song playing in Spotify, YouTube Music, YouTube or Apple Music and applies a matching tone. You can customise every genre curve.
- **Headphone correction.** It has 6,000+ AutoEQ profiles. It recognises Bluetooth, USB-C and wired headphones and remembers your choice per device.
- **Genre strength:** choose how strongly genre EQ shapes the sound.
- **My devices:** give each pair of headphones, the car and the phone speaker their own sound.
- **Sound layers:** see exactly what EQify changes, with a plain-language summary.
- **Your week in sound:** genres, top artists and a shareable card.
- **Manual 8-band EQ** with your own presets, which you can share as codes, files or QR codes.
- **Bass boost and output protection** (a limiter) so boosts don't clip, with optional easing at high volume and a bass button in the notification.
- **Backup and restore** of presets, genre curves, devices and settings to one file.
- **Loudness compensation** for full sound at low volume, and an optional **volume limit**.
- **Sleep timer** that fades the music out, plus **test sounds** (left, right, sweep).
- **Home screen widget**, app-icon shortcuts and **Tasker** support.
- Works in **landscape and on tablets**.
- **Safe listening** reminders based on WHO guidance, **stereo balance**, a **live spectrum**, and **AutoEQ ParametricEQ** import.
- A **Wear OS** remote (optional, separate APK).
- **Themes**, and Quick Settings tiles for EQ, Bass and the Sleep timer.
- **Update alerts** in the app, plus automatic updates through Obtainium.
- **No account, no ads, no analytics.** See the [privacy policy](PRIVACY.md).

Requires Android 8.0 or later.

## Install

### Option 1: Obtainium (recommended, gets automatic updates)

[Obtainium](https://github.com/ImranR98/Obtainium) installs apps straight from GitHub Releases and keeps them updated.

1. Install Obtainium from its [releases page](https://github.com/ImranR98/Obtainium/releases).
2. In Obtainium, tap **Add app** and paste:
   ```
   https://github.com/parthsharma365628/eqify-releases
   ```
3. Tap **Add**, then **Install**. Obtainium will tell you when a new version is out.

Beta versions are marked as pre-releases. If Obtainium says it found no release, open EQify's settings in Obtainium and turn on **Include prereleases**.

### Option 2: Download the APK

1. Open the [latest release](../../releases) and download `EQify-<version>.apk`.
2. Open the file and allow **Install unknown apps** for your browser or file manager when asked.

### Wear OS watch (optional)

The watch app is a remote for EQify on your phone: Pause, Bass and the sleep timer.

1. Download `EQify-Wear-<version>.apk` from the same release.
2. Install it on the watch. Turn on **Developer options → ADB debugging** and **Debug over Wi-Fi** on the watch, then run `adb connect <watch IP>` and `adb install EQify-Wear-<version>.apk`.
3. Open EQify on the watch while EQify is running on the phone.

### Before and after installing

- **Uninstall older EQify builds first**, so two equalizers don't compete.
- **Play Protect warning.** EQify isn't on the Play Store, so Play Protect may call it unsafe or ask you to scan it. Tap **More details**, then **Install anyway**. You don't need to turn Play Protect off.
- **Notification access (optional).** It lets EQify detect the song you play. Android's dialog says the app could read, dismiss and reply to notifications, because that's how Android describes this one permission. EQify only reads the song title and artist from the four music apps above. It never reads, dismisses or replies to any other notification. You can skip it: presets, headphone correction and bass still work.
- **If the notification access switch is greyed out** (Android 13 and later): open **Settings → Apps → EQify**, tap the **⋮** menu, choose **Allow restricted settings**, confirm with your PIN, then turn access on again.

## Feedback

- **In the app:** Settings → Send feedback. Your app version and phone model are filled in for you.
- **On GitHub:** [open an issue](../../issues/new/choose) for bugs or ideas.

When reporting a bug, please include your phone model, Android version, music app and headphones.

## About

Made by Parth Sharma and Shreyansh Mangal. EQify is closed source; this repository only hosts releases, the privacy policy and issue tracking.

Headphone correction data is derived from [AutoEq](https://github.com/jaakkopasanen/AutoEq) (MIT License, © Jaakko Pasanen). EQify is not affiliated with or endorsed by AutoEq or the measurement providers. Other third-party licences are listed in the app under Settings → Open-source licences.

Copyright © 2026 Parth Sharma and Shreyansh Mangal. All rights reserved.
