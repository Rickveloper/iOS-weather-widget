# Lock Screen Weather Widget

<p align="center">
  <img src="./lockscreen-banner.PNG" alt="Lock Screen Weather Banner" width="100%" style="border-radius:8px;" />
</p>

**A GPS-powered weather widget for Scriptable, made for iOS Lock Screens.**  
Stay updated with hyperlocal, emoji-coded forecasts that match the vibe of your day.

---

<p align="center">
  <img src="https://img.shields.io/badge/Built%20With-JavaScript-yellow?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Made%20For-Scriptable-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/github/license/Rickveloper/iOS-weather-widget?style=for-the-badge"/>
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

> Store both scripts inside Scriptable.

### 3. Shortcut + Automation (Optional but Recommended)

<p align="center">
  <img src="./shortcut-example.jpg" alt="Shortcut Setup Example" width="85%" />
</p>

1. Open the **Shortcuts** app  
2. Create a shortcut:  
   - Action: **Run Script**  
   - Script: `Update Weather Location`  
3. Add it to your Lock Screen as a tap-to-refresh shortcut

You can also automate location updates:

<p align="center">
  <img src="./automation-example.jpg" alt="Automation Example" width="85%" />
</p>

- Set it to run **when Scriptable opens** or on a schedule (e.g. every hour)

---

## Widget Demo

<p align="center">
  <img src="./widget-demo.PNG" alt="Weather Widget Demo" width="75%" />
</p>

---

## File System

| File                      | Purpose                               |
|---------------------------|----------------------------------------|
| `weather-loc.json`        | Stores GPS + timestamp for accuracy   |
| `Lockscreen Weather.js`   | Widget display script                  |
| `Update Weather Location.js` | Location grabber (runs silently)    |

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
