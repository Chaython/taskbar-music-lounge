# Taskbar Music Lounge

A media controller that uses Windows 11 native DWM styling for a seamless look.

### 🛠️ Fork Changelog (v4.2.5)
* **Fixed:** Instant widget appearance when taskbar auto-hide reveals (bypasses debounce).
* **Fixed:** App opening fallback now uses case‑insensitive substring matching (fixes Edge, Spotify, etc.).
* **Fixed:** Progress bar now spans the full width of the panel.
* **Fixed:** Duration now uses MaxSeekTime as fallback.
* **Fixed:** Startup flashing when the taskbar is auto-hidden.
* **Fixed:** Added 500 ms debounce only for startup / taskbar size changes.
* *Modifications by Chaython.*

## 🚀 v3 vs v4: Major Architecture Shift
| Feature | v3 (Legacy) | v4 (Current) |
| :--- | :--- | :--- |
| **Performance** | Polling Loop (High CPU wakeups) | **Event-Driven** (0% CPU when idle) |
| **Smoothness** | 1-second delay on moves | **Instant** sync with Taskbar animations |
| **Compatibility** | Chrome/Spotify only | **Universal** supports all media players |
| **Visuals** | Square Art, Fixed Size | **Rounded Art**, 4K Scalable Icons, Acrylic Blur, Rounded Art |
| **Behavior** | Always visible (Clunky) | **Smart Auto-Hide** Hides on fullscreen (Idle, Games, Taskbar Hide) |

## ✨ Features
* **Universal Support:** Smart scanning detects active playback from any app, not just the "focused" one.
* **Album Art:** Displays current track cover art.
* **Fullscreen Mode:** Hides automatically when running full-screen applications.
* **Native Look:** Uses Windows 11 hardware-accelerated rounding and acrylic blur.
* **Idle Timeout:** Optional setting to fade out the widget when music is paused for X seconds.
* **Controls:** Play/Pause, Next, Previous.
* **Volume:** Scroll over widget to adjust volume.
* **Progress Bar:** Shows playback position when available.
* **Open App:** Click on the empty area to bring the playing app to the front.

## ⚠️ Requirements
* **Disable Widgets:** Taskbar Settings -> Widgets -> Off.
* **Windows 11:** Required for rounded corners.
