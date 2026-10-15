# Taskbar Music Lounge

A media controller that uses Windows 11 native DWM styling for a seamless look.

### 🛠️ Fork Changelog (v4.3.1)
* **Fixed:** Memory leak / constant-calling when taskbar auto-hides at rest.
* **Fixed:** Widget no longer leaves a visible "lip" when the taskbar auto-hides.
* **Fixed:** Resolved visibility loop bugs causing flickering.
* **Fixed:** Added DPI scaling support for hidden taskbars (4K monitor fix).
* **Added:** Adaptive Color — tint the panel background from album art.
* **Fixed:** Removed unused <vector> and <atomic> headers.
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

<!-- chaython-funding:start -->
## Support development

[GitHub Sponsors](https://github.com/sponsors/Chaython) · [Patreon](https://patreon.com/Chaython) · [Buy Me a Coffee](https://buymeacoffee.com/chaython) · [PayPal](https://paypal.me/ChaythonM)

Crypto donations:

- ETH (Ethereum): `0x201B6E0B0282BBAE1592C24f9CbD39009A70F7d7`
- BTC (Bitcoin): `32o7JmXgFcs4R1SbcLLVKQCRw9KHkhneJi`
- SOL (Solana): `BDicyUL9zizDeYBLw8oBwotv6jtHotLLQD7Bcqg2atLk`
- **USDC (Base network):** `0xBeD35dcAd9F1A32459B3C0DF004371EBE939E760`

**Send USDC only on Base.**
<!-- chaython-funding:end -->
