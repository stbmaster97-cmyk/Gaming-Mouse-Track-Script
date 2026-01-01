# 🎮 Gaming Mouse Track.
**Global Canvas Interaction & Stabilized Source Tracking for Gaming.**

`Gaming Mouse Track v2.4` is a versatile Lua script for OBS Studio that bridges the gap between your mouse and your stream's canvas. Designed for gaming and professional tutorials, it allows any source—regardless of its resolution or size—to dynamically follow your cursor.

[![Watch the video]](https://youtu.be/eX2jvM8XAiE?si=qzD1at-zKMlYHJsm)
---

## ✨ Core Features

* **Global Canvas Adaptability:** Works seamlessly across multiple canvases. Whether your source is the same size as your stream, game, source or a smaller windowed element, the tracking scales to fit.
* **Multi-Source Support:** Independent settings for up to **10 different sources** simultaneously. You can have your gameplay, Window, and browser all tracking at once with unique speeds.
* **Dual-Filter Logic:** Automatically manages **Crop + Scale** filters to ensure a 100% canvas fill—no black bars, even when the source resolution doesn't match the output.
* **Zoom:** Use a hotkey to instantly "punch in" on a specific area for a sniper-cam or detail-focused effect.

---

## 🕹️ Specialized Gaming Logic

* **Anti-Jitter (Movement Threshold):** In many games, the crosshair or center-point isn't perfectly still due to idle sway or breathing animations. The script ignores these micro-movements (customizable in pixels), ensuring your stream remains rock-steady until you actually move your mouse.
* **Deadzone Buffers:** Create a "safe zone" in the center of your screen. The camera won't move while your mouse is inside this area, preventing motion sickness for viewers during small aim adjustments.
* **Smart Inventory Toggle (Auto-Disable):** Designed for games where the "Interact" key is the same as the "Inventory" key. This feature prevents the tracker from staying active in a menu if triggered by a multi-use key, automatically disabling and centering after a short idle period.
* **Intelligent Auto-Reset:**
    * **On-Screen Idle Reset:** Automatically returns the view to center if the mouse stops moving for a set duration.
    * **Boundary Safety:** If you flick your mouse to a second monitor or out of the game window, the camera instantly snaps back to center.

---

## 🛠️ Configuration & Settings

| Setting | Gamer's Use Case |
| :--- | :--- |
| **Movement Threshold** | **15-25px** — Prevents the camera from twitching due to in-game crosshair "wiggle." |
| **Deadzone %** | **5-10%** — Creates a center "safe zone" for micro-aiming without moving the camera. |
| **Auto-Disable Time** | **1-2 sec** — Safely toggles tracking off after you finish looting or navigating menus. |
| **Center on Stop** | **Enabled** — Automatically centers your view the moment tracking is disabled. |
| **Tracking Speed** | **40-60%** — Balances responsiveness with smooth, cinematic movement. |

---

## 🚀 Installation & Usage

1. **Download** the `Gaming Mouse Track v2.4.lua` file.
2. Open OBS Studio and go to **Tools** -> **Scripts**.
3. Click the **+** button and select the script.
4. **Setup Hotkeys:** Go to **Settings -> Hotkeys** to assign:
    * `Toggle / Enable Mouse Tracking`
    * `Toggle Zoom Level`
    * `Reset Tracker Position` (Manual snap-back to center)

---

## ⚠️ Technical Notes
* **Zoom Rescaling:** Note that version 2.4 has a known visual offset bug during high-multiplier zooming which is being addressed in the next update.
* **Filter Management:** The script manages "Track_P" and "Stretch_P" filters automatically. Manual changes to these filters may be overwritten.
