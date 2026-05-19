<div align="center">

# 🎮 GBP-Downloader
### Receive Game Boy Camera photos straight in your browser.

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](./LICENSE)
[![GitHub Pages](https://img.shields.io/badge/demo-live-brightgreen.svg)](https://hexlions.github.io/GBP-Downloader/gbp_downloader.html)
[![Web Serial](https://img.shields.io/badge/Web%20Serial-API-orange.svg)](https://developer.mozilla.org/en-US/docs/Web/API/Web_Serial_API)
[![No Install](https://img.shields.io/badge/install-not%20required-success.svg)](#)
[![Version](https://img.shields.io/badge/version-1.5-purple.svg)](#)

**🌐 [Open the app →](https://hexlions.github.io/GBP-Downloader/gbp_downloader.html)**

</div>

---

## 🤔 What is this?

A single-page web tool for receiving photos from the **Game Boy Printer Emulator**. No installation, no build step, no serial monitor — just open the page, plug in your Arduino, and print.

---

## ✨ Features

- 🚀 **Zero install** — runs entirely in the browser, single HTML file
- 🔌 **Web Serial** — direct USB communication, no drivers needed
- 📦 **Offline-first** — load once, works without internet
- 🖼️ **Native PNG export** — single photos or batch ZIP (1× / 2× / 4× / 8×)
- 🎨 **22 palettes** — emulators, hardware-accurate, GBC modes, community favorites, and classics
- 🖌️ **Custom palette** — paste any palletizer string (`#aaa #bbb #ccc #ddd palletizer Name`)
- 🔲 **Dithering** — Bayer 4×4 ordered dither for smoother gradients
- 📐 **Gamma correction** — γ=2.2 curve to simulate the real DMG screen response
- 🕹️ **DMG-themed UI** — grey plastic shell, purple DOT MATRIX stripe, magenta buttons

---

## 🚀 Quick Start

### What you need

- 🌐 A Chromium browser (Chrome, Edge, Brave, Opera, Arc…)
- 🤖 An Arduino Nano or Uno with the [GBP Emulator firmware](https://github.com/mofosyne/arduino-gameboy-printer-emulator) flashed
- 🎮 A Game Boy + Link Cable wired to the Arduino
- 📷 A Game Boy Camera (or any printable GB game)

### Step-by-step

```
┌─────────────────────────────────────────────────────────┐
│  1. 🔌 Plug the Arduino into USB                         │
│  2. 🎮 Connect the Game Boy via Link Cable               │
│  3. 🌐 Open the app → click Connect                      │
│  4. 🖨️  Print from the Game Boy                          │
│  5. 🖼️  Save photos as PNG or download all as ZIP        │
└─────────────────────────────────────────────────────────┘
```

> 💡 **Need to flash the firmware?** Grab the `.hex` from [mofosyne/arduino-gameboy-printer-emulator](https://github.com/mofosyne/arduino-gameboy-printer-emulator) and use the Arduino IDE or `avrdude`.

---

## 🎨 Palettes

22 palettes organised in 5 groups:

| Group | Palettes |
|---|---|
| **Emulators** | BGB, DMG, SameBoy, Gambatte |
| **Hardware accurate** | Accurate (DMG-01 sampled), NSO, Pocket, GB Light |
| **GBC color modes** | GBC Green, GBC Red, GBC Blue, GBC Gray |
| **Community** | Kirokaze, Mist, Wishes, Hollow, 2-Bit |
| **Classic** | B&W, Sepia, Noir, Ice, Burn |

You can also paste any **palletizer string** directly in the sidebar to create a custom palette:

```
#dbf4b4 #abc396 #7b9278 #4c625a palletizer My Custom Palette
```

---

## 📁 Project structure

```
GBP-Downloader/
├── gbp_downloader.html    ← the app (v1.5)
├── index.html             ← redirect to downloader
├── README.md
├── LICENSE                ← GPL-3.0
└── .gitignore
```

---

## 🙏 Credits

This project stands on the shoulders of an amazing open-source community:

- 🔧 **[mofosyne/arduino-gameboy-printer-emulator](https://github.com/mofosyne/arduino-gameboy-printer-emulator)** — the Arduino firmware that makes it all possible
- 🖼️ **HerrZatacke**, **BjornB2**, **virtuaCode** — pioneering work on JS-based Game Boy Printer decoding
- 🎨 **Raphaël Boichot** — protocol research and compression support
- 🗺️ **West McGowan** — wiring documentation

---

## 📜 License

Released under the **[GNU General Public License v3.0](./LICENSE)** — same as the upstream firmware, keeping the whole ecosystem fully open and free.

> This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

---

<div align="center">

**Made with 💚 by [HexLions](https://github.com/HexLions)** · *Florence, Italy* 🇮🇹

*If this helped you, drop a ⭐ on the repo!*

</div>
