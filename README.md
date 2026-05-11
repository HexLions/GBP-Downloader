<div align="center">

# 🎮 GBP-Downloader

### Receive Game Boy Camera photos. Flash the firmware. All in your browser.

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](./LICENSE)
[![GitHub Pages](https://img.shields.io/badge/demo-live-brightgreen.svg)](https://hexlions.github.io/GBP-Downloader/gbp_downloader.html)
[![Web Serial](https://img.shields.io/badge/Web%20Serial-API-orange.svg)](https://developer.mozilla.org/en-US/docs/Web/API/Web_Serial_API)
[![No Install](https://img.shields.io/badge/install-not%20required-success.svg)](#)

**🌐 [Open the app →](https://hexlions.github.io/GBP-Downloader/gbp_downloader.html)**

</div>

---

## 🤔 What is this?

Two single-page web tools for the **Game Boy Printer Emulator** ecosystem. No installation, no build step, no `avrdude`, no Arduino IDE. Just open the page, plug in your Arduino, and go.

| 📥 Downloader | ⚡ Flasher |
|:---:|:---:|
| Receive photos from your Game Boy Camera | Flash the GBP Emulator firmware |
| Decodes 2bpp tile data → PNG | STK500v1 protocol over Web Serial |
| Export single PNG or ZIP | Works on Arduino Nano / Uno |

---

## ✨ Features

- 🚀 **Zero install** — runs entirely in the browser
- 🔌 **Web Serial** — direct USB communication, no drivers needed
- 📦 **Offline-first** — load once, works without internet
- 🖼️ **Native PNG export** — single photos or batch ZIP
- 🛠️ **Browser-based flasher** — no Arduino IDE required
- 🎨 **DMG-themed UI** — green-tinted nostalgia included

---

## 🚀 Quick Start

### What you need

- 🌐 A Chromium browser (Chrome, Edge, Brave, Opera, Arc...)
- 🤖 An Arduino Nano or Uno
- 🎮 A Game Boy + Link Cable wired to the Arduino
- 📷 A Game Boy Camera (or any printable GB game)

### Step-by-step

```
┌─────────────────────────────────────────────────────────┐
│  1. ⚡  Open the FLASHER page                            │
│  2. 🔌 Plug in the Arduino via USB                      │
│  3. 📂 Select the firmware .hex file → click FLASH       │
│  4. 🎮 Connect Game Boy to Arduino via Link Cable        │
│  5. 📥 Open the DOWNLOADER page → click Connect          │
│  6. 🖨️  Print from the Game Boy                          │
│  7. 🖼️  Save photos as PNG or download all as ZIP        │
└─────────────────────────────────────────────────────────┘
```

---

## 📁 Project structure

```
GBP-Downloader/
├── gbp_downloader.html    ← receive & decode photos
├── gbp_flasher.html       ← flash firmware in-browser
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
- 📡 **STK500v1 protocol** — adapted for Web Serial flashing

---

## 📜 License

Released under the **[GNU General Public License v3.0](./LICENSE)** — same as the upstream firmware, keeping the whole ecosystem fully open and free.

> This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

---

<div align="center">

**Made with 💚 by [HexLions](https://github.com/HexLions)** · *Florence, Italy* 🇮🇹

*If this helped you, drop a ⭐ on the repo!*

</div>
