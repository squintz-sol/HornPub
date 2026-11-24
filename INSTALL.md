# Installing HornPub

## 1. Download

Go to [Releases](https://github.com/squintz-sol/HornPub/releases) and download
`HornPub-v<version>-Full-Windows.zip` from the newest release's *Assets*.

## 2. Unzip

Right-click the zip, choose **Extract All…**, and extract it to a folder of your choice (for example
`Documents\HornPub`).

- Keep `HornPub.exe` next to its `_internal` folder; the app needs both.
- Don't run HornPub from inside the zip without extracting it.

## 3. Run

Double-click `HornPub.exe`.

Windows SmartScreen may show *"Windows protected your PC"*. HornPub isn't code-signed, so Windows doesn't
know the publisher. Click **More info → Run anyway**, but only for a zip you downloaded from this project's
Releases page.

Nothing else needs to be installed (Windows 10 or 11, 64-bit). On first launch, HornPub creates an empty data
folder for your recordings and settings at `%LOCALAPPDATA%\MapleGrind`.

## 4. Set up the game

- Play in **windowed or borderless** mode on your **main monitor**.
- Keep the **status bar** (level and EXP), the **minimap**, and the **quickslot** with your potions visible.
- Open your **inventory** once at the start, so HornPub can read your mesos.

## 5. Record a session

| Action         | Button        | Default hotkey |
|----------------|---------------|----------------|
| Start          | Start         | Shift+F7       |
| Pause / Resume | Pause         | Shift+F8       |
| Stop and save  | Stop          | Shift+F9       |

- Pause while you're shopping or on a break, so that time doesn't count.
- After Stop, the dashboard keeps showing the recording. **Clear** empties the dashboard; the recording stays
  in **History**.
- Change the hotkeys in **⚙ Settings → Hotkeys**. *Save and test…* checks that they reach HornPub while the
  game is in front.

## 6. Potions (one-time setup)

HornPub ships without any game artwork, so it doesn't know your potion icons yet. The first time it sees one,
the HP / MP area shows **"identify N items"**. Click it, then pick the potion for each icon (or *Not a potion*
for pet food, scrolls and the like). HornPub remembers your choice. Set a potion's NPC price with the pencil
in the potion list; Net Mesos uses it.

## 7. Map pictures

Open your minimap on a map once while recording, and HornPub saves a small picture of it for History and the
Top 3 cards. After about 10 minutes on a map with no picture, a quiet reminder appears on the dashboard
(Settings → Reminders can turn it off).

## Updating

Download the new zip and extract it to a new folder, or over the old one once HornPub is closed. Your
recordings and settings are kept, because they live in `%LOCALAPPDATA%\MapleGrind`, not in the app folder.

## Uninstalling

Delete the HornPub folder. To also remove your recordings and settings, delete `%LOCALAPPDATA%\MapleGrind`.

## Check your download (optional)

Each release lists the zip's SHA-256 checksum. In PowerShell:

```powershell
Get-FileHash .\HornPub-v0.3.10-Full-Windows.zip -Algorithm SHA256
```

The hash should match the one on the release page.
