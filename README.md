# Lock Screen Weather Widget

<p align="center">
  <img src="./A9E0459B-A18E-45E8-817A-B50A0EAACA75.png" alt="Lock Screen Weather Banner" width="100%" style="border-radius:8px;" />
</p>

**A GPS-powered weather widget for Scriptable, made for iOS Lock Screens.**  
Stay updated with hyperlocal, emoji-coded forecasts that match the vibe of your day.

---

<p align="center">
  <img src="https://img.shields.io/badge/Built%20With-JavaScript-yellow?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Made%20For-Scriptable-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/github/license/Rickveloper/lockscreen-weather?style=for-the-badge"/>
</p>

---

## Features

- **Live Temperature** in °F (via Open-Meteo)
- **Emoji Forecast** matching weather vibes
- **Location-Aware**: Automatically grabs city/state
- **Vibe Reading**: Describes the weather in real language (e.g. _Cold AF_)
- **Timestamp**: Shows last updated time
- **Designed for iOS**: Centered, clean, Lock Screen-ready

---

## Setup

### 1. Prerequisites

- [Scriptable App](https://apps.apple.com/us/app/scriptable/id1405459188)
- iOS 16+ with Lock Screen widget support

### 2. Scripts to Add

| Script Name              | Description                         |
|--------------------------|-------------------------------------|
| `Lockscreen Weather`     | Displays the widget                 |
| `Update Weather Location`| Gets your current location silently |

> Save both scripts in the Scriptable app

### 3. Shortcut Automation (Optional but Recommended)

Keep your widget fresh with a background automation and manual trigger.

1. Open the **Shortcuts** app  
2. Create a shortcut:  
   - **Action**: Run Script  
   - **Script**: `Update Weather Location`  
3. (Optional) Add it to your Lock Screen as a tap-to-refresh shortcut  
4. (Optional) Add an Automation:  
   - **Trigger**: When Scriptable is opened  
   - **Action**: Run `Update Weather Location`

<p align="center">
  <img src="./D28DA2EE-C4D4-4472-ABF5-91D163B3553D.jpeg" alt="Shortcut Automation Example" width="75%" />
</p>

### 4. Add the Widget

- Long-press your Lock Screen → **Customize**
- Add a **Scriptable** widget → Choose `Lockscreen Weather`

---

## File System

| File                         | Purpose                               |
|------------------------------|----------------------------------------|
| `weather-loc.json`           | Stores GPS + timestamp for accuracy   |
| `Lockscreen Weather.js`      | Widget display script                  |
| `Update Weather Location.js` | Location grabber (runs silently)      |

---

## Demo

<p align="center">
  <img src="./0833DAE2-CCCD-42B7-B184-0B982ED74EBF.jpeg" alt="Lock Screen Weather Demo" width="75%" />
</p>

---

## APIs Used

- [Open-Meteo Weather API](https://open-meteo.com/)
- [Nominatim Reverse Geocoding](https://nominatim.org/release-docs/latest/api/Reverse/)

---

## License

[MIT](./LICENSE) — Free to remix, build on, or launch from

---

## Credits

Built with cold hands and a hot idea by [@Rickveloper](https://github.com/Rickveloper)

---

## Coming Soon

- Light/dark theme toggle
- Temperature in °C
- Weather alerts
- Home screen widget version
- Animated icons