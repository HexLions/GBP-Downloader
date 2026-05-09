# GBP Downloader

A single-file web app to **receive and save photos from your Game Boy Camera** via an Arduino running the Game Boy Printer Emulator firmware.

```
┌──────────────┐
│  ░░░░░░░░░░  │
│  ░░GAMEBOY░░ │     open gbp_downloader.html in Chrome / Edge
│  ░░░░░░░░░░  │     connect Arduino → press print → save photos
│  ▓▓ ▓▓  ◊ ◊  │
└──────────────┘
```

## Features

- Connects to your Arduino over **Web Serial** (Chrome / Edge / Opera, desktop only)
- Decodes the V3 raw packet stream with **RLE decompression** (Pokémon TCG and other compressed-mode games)
- 8 selectable palettes — **BGB** default, DMG, BW, Pocket, Sepia, Noir, Ice, Burn
- **Auto-connect** to remembered devices on page load and on cable plug-in
- **Auto-download** PNGs on every print (optional), camera-shutter sound
- Export 1× / 2× / 4× / 8× PNGs or batch **ZIP** the whole gallery
- Drag & drop `.txt` / `.log` hex captures for offline decoding
- Zero dependencies — single HTML file, works fully offline

## Quick start

```bash
git clone https://github.com/HexLions/gbp-downloader.git
# open index.html in Chrome / Edge / Opera
```

Or use the live GitHub Pages version:
> https://hexlions.github.io/gbp-downloader/

## Setup

1. Flash your Arduino with the [Game Boy Printer Emulator firmware](https://github.com/mofosyne/arduino-gameboy-printer-emulator)
2. Wire the Arduino to a Game Boy link cable (pinout in the upstream README)
3. Open `gbp_downloader.html`, click **CONNECT TO ARDUINO**
4. Press print on your Game Boy — photos appear instantly in the gallery

## Browser support

Requires the **Web Serial API** — available in Chrome, Edge and Opera on desktop.
Not supported in Firefox, Safari, or any mobile browser.

On Linux, add your user to the `dialout` group:
```bash
sudo usermod -aG dialout $USER
```

## Credits

The Arduino firmware this tool connects to is the work of:

- **Brian Khuu** ([@mofosyne](https://github.com/mofosyne)) — original author & maintainer
- **Raphaël Boichot** — protocol research, compression & fast-mode support
- **HerrZatacke** — WebUSB integration & [gb-printer-web](https://github.com/HerrZatacke/gb-printer-web)
- **BjornB2** & **virtuaCode** — JS decoder improvements and color palettes
- **West McGowan** — wiring documentation

Firmware: <https://github.com/mofosyne/arduino-gameboy-printer-emulator> (GPL-3.0)

## License

MIT — see `LICENSE`.
The Arduino firmware flashed to your board is GPL-3.0 © its authors (see Credits).
