# HornPub

**Free MapleStory Classic World EXP & Farming Tracker for Windows**

HornPub watches your game screen while you train and tells you how your session is going: EXP per hour,
time to your next level, mesos per hour, potions used, and which maps are your best farming spots. It only
reads what is visible on your screen.

> HornPub is an independent fan project. It is not affiliated with, endorsed or sponsored by NEXON.
> See [DISCLAIMER.md](DISCLAIMER.md).

## Download

**[Download the latest version from Releases](https://github.com/squintz-sol/HornPub/releases)**. Pick
`HornPub-v<version>-Full-Windows.zip` under *Assets*.

HornPub is free. GitHub Releases is its only official download location: don't download it from anywhere
else, and never pay for it. Each release lists the zip's SHA-256 checksum so you can check your download
([how](INSTALL.md#check-your-download-optional)).

The current version is a **pre-release**: it works, but it is still being tested on more PCs and screen sizes.

## Features

- **EXP tracking:** EXP gained, EXP per minute and per hour, and level-ups handled correctly.
- **Rolling EXP/hour:** your rate over the last 10 minutes (choose 5, 10, 15 or 30). After you stop, the final
  rolling rate is kept, and the whole-session average is still available.
- **Level-up ETA and custom targets:** the time left and the local clock time you'll reach your next level, or
  any EXP % you choose.
- **Mesos tracking:** mesos gained and mesos per hour.
- **Potion counting:** HP / MP potions used and picked up, read from your quickslot. You name each potion icon
  once with *Identify…* and HornPub remembers it.
- **Net Mesos:** mesos earned after the cost of the potions you drank (an estimate; see
  [Known limitations](#known-limitations)).
- **History:** every recording is saved on your PC, with an EXP chart, notes, renaming, and trimming (cut off
  time spent in town).
- **Top 3 Farming Maps:** your best maps ranked by EXP/hr, Mesos/hr or Net Mesos/hr (best recording or average).
- **Map Performance filters:** by map and period (today, last 7 / 30 days, or a custom range).
- **Minimap thumbnails:** each map gets a picture from its minimap the first time you open the minimap there.
- **Customizable hotkeys:** Start / Pause / Stop with Shift+F7 / F8 / F9 by default; change or disable them.
- **Help / Getting Started:** a short built-in guide (the ⓘ button next to Settings).
- **CSV export** of all your recordings.

## Requirements

- Windows 10 or 11 (64-bit). Nothing else to install; Python is not needed.
- MapleStory Classic World in **windowed or borderless** mode on your **main monitor**.
- The status bar, the minimap and the quickslot visible on screen.

## Quick start

1. Download the zip from [Releases](https://github.com/squintz-sol/HornPub/releases) and unzip the whole
   `HornPub` folder (for example into `Documents\HornPub`).
2. Run `HornPub.exe`. Windows SmartScreen may warn you because the app isn't code-signed: choose
   *More info → Run anyway*.
3. In the game, open your inventory once (so HornPub can read your mesos), then press **Start**
   (or Shift+F7).

Full instructions: [INSTALL.md](INSTALL.md).

## Privacy and fair play

- HornPub only takes screenshots of your monitor and reads the numbers on them.
- It **never** reads or changes the game's memory, injects nothing, intercepts no network traffic, and sends no
  keys or clicks to the game.
- It does not go online. Your recordings and settings stay on your PC, in `%LOCALAPPDATA%\MapleGrind`.

## Known limitations

- **Screen reading is an estimate.** Accuracy depends on your screen resolution and UI size, on the status bar,
  minimap and quickslot being visible and uncovered, and on text recognition (OCR). A number can occasionally
  be misread; HornPub checks values against each other and skips readings it doesn't trust.
- **Potions are counted from the quickslot only.** A potion that isn't on your quickslot isn't counted, and
  HornPub can't see every potion use. For example, potions used while the quickslot is hidden or covered are
  missed.
- **Net Mesos is an estimate.** HornPub doesn't see NPC purchases and sales individually. A big jump in a
  potion count is treated as a possible restock and left out of farming earnings rather than guessed.
- **Map names** are read from the minimap and can be misread; you can correct them in History.
- **Main monitor only.** Multi-monitor setups and unusual UI scales are less tested.
- The app isn't code-signed, so Windows may warn you the first time you run it.

## Reporting problems

Open an [issue](https://github.com/squintz-sol/HornPub/issues). If something is read wrong, say what the game
showed and what HornPub showed. Screenshots of both help; crop out your character name if you like.

## Release history

See [RELEASES.md](RELEASES.md).

## License

HornPub is **closed-source freeware**: free to download and use, but all rights reserved. Don't sell,
re-upload, modify or decompile it. This repository contains only documentation; the source code isn't public.
The open-source libraries bundled with the app keep their own licences, listed in `THIRD_PARTY_NOTICES.txt`
inside the download.
