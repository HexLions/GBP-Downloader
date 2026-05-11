<div align="center">

# 🎮 GBP-Downloader

### Receive Game Boy Camera photos straight in your browser.

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](./LICENSE)
[![GitHub Pages](https://img.shields.io/badge/demo-live-brightgreen.svg)](https://hexlions.github.io/GBP-Downloader/gbp_downloader.html)
[![Web Serial](https://img.shields.io/badge/Web%20Serial-API-orange.svg)](https://developer.mozilla.org/en-US/docs/Web/API/Web_Serial_API)
[![No Install](https://img.shields.io/badge/install-not%20required-success.svg)](#)

**🌐 [Open the app →](https://hexlions.github.io/GBP-Downloader/gbp_downloader.html)**

</div>

---

## 🤔 What is this?

A single-page web tool for receiving photos from the **Game Boy Printer Emulator**. No installation, no build step, no serial monitor — just open the page, plug in your Arduino, and print.

---

## ✨ Features

- 🚀 **Zero install** — runs entirely in the browser
- 🔌 **Web Serial** — direct USB communication, no drivers needed
- 📦 **Offline-first** — load once, works without internet
- 🖼️ **Native PNG export** — single photos or batch ZIP
- 🎨 **DMG-themed UI** — green-tinted nostalgia included

---

## 🚀 Quick Start

### What you need

- 🌐 A Chromium browser (Chrome, Edge, Brave, Opera, Arc...)
- 🤖 An Arduino Nano or Uno with the [GBP Emulator firmware](https://github.com/mofosyne/arduino-gameboy-printer-emulator) already flashed
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

## 📁 Project structure

```
GBP-Downloader/
├── gbp_downloader.html    ← the app
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

---

## 📜 License

Released under the **[GNU General Public License v3.0](./LICENSE)** — same as the upstream firmware, keeping the whole ecosystem fully open and free.

> This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

---

<div align="center">

**Made with 💚 by [HexLions](https://github.com/HexLions)** · *Florence, Italy* 🇮🇹

*If this helped you, drop a ⭐ on the repo!*

</div>
