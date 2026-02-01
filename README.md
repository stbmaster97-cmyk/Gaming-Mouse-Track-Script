# 🖱️ Gaming Mouse Track
Check right side of this page download last release V2.7.\
USE Source Clone by Exeldro to use the vertical presets or it will crop your original source.

### **Multiple source mouse tracker with canvas limits for Gaming and Vertical streams​**

`Gaming Mouse Track` is a high-performance Lua script for OBS Studio designed to bridge the gap between your mouse movements and your stream's canvas. Whether you are hitting clips in an FPS or hosting professional tutorials, this script ensures your sources follow your cursor with surgical precision.

[![Watch the video]](https://www.youtube.com/watch?v=lxAwY-MRef4)
---

## 🚀 Core Features

* 🌍 **Global Canvas Adaptability:** Works seamlessly across multiple canvases. Tracking scales perfectly whether your source matches your stream size or is a smaller windowed element.
* 🔢 **Multi-Source Support:** Take full control with independent settings for up to **10 different sources** simultaneously.
* 📐 **Dual-Filter Logic:** Automatically manages **Crop + Scale** filters to ensure a 100% canvas fill—no black bars, even when resolutions don't match.
* 🔍 **Instant Zoom:** Assign a hotkey to "punch in" on specific areas for high-detail focus or a "sniper-cam" effect.

---

## 🎮 Specialized Gaming Logic

* 🛤️ **Tracking Modes**
    * **Both:** Full axis tracking (Standard).
    * **Horizontal Only:** Locks vertical axis; follows left-to-right movements only.
    * **Vertical Only:** Locks horizontal axis; follows up-and-down movements only.
* ⚖️ **Anti-Jitter (Movement Threshold):** Ignores micro-movements (customizable in pixels) caused by in-game breathing or shaky hands.
* 🛡️ **Deadzone Buffers:** Create a "safe zone" in the center. The camera stays still while your mouse is inside this area, preventing motion sickness during micro-aiming.
* 🎒 **Smart Inventory Toggle:** Perfect for games where "Interact" and "Inventory" share a key; it auto-disables and centers the camera after a short idle period.
* 🔄 **Intelligent Auto-Reset**
    * **On-Screen Idle:** Returns to center if the mouse is stationary for a set duration.
    * **Boundary Safety:** Snaps back to center if the mouse leaves the game window or monitor.

---

## ⚙️ Configuration & Settings

| Setting | Gamer's Recommended Use Case |
| :--- | :--- |
| **Tracking Mode** | Choose **Both**, **Horizontal**, or **Vertical** for axis-locking. |
| **Movement Threshold** | **15-25px** — Prevents twitching from crosshair "wiggle." |
| **Deadzone %** | **5-10%** — A "safe zone" for micro-aiming stability. |
| **Auto-Disable Time** | **1-2 sec** — Safely toggles tracking off after looting. |
| **On-Screen Idle Reset** | Duration of stillness required before the camera auto-centers. |
| **Tracking Speed** | **40-60%** — Balances responsiveness with cinematic smoothness. |

---

## 📥 Installation & Usage

1. **Download** the `Gaming Mouse Track.lua` file last version.
2. Open **OBS Studio** and navigate to `Tools` -> `Scripts`.
3. Click the **+** button and select the downloaded file.
4. **Assign Hotkeys:** Go to `Settings` -> `Hotkeys` to set:
    * `Toggle / Enable Mouse Tracking`
    * `Toggle Zoom Level`
    * `Reset Tracker Position` (Manual snap-to-center)

---

## ⚠️ Technical Notes

> USE Source Clone by Exeldro to use the vertical presets or it will crop your original source
   
---
