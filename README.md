# Need For Speed™ II SE — Windows 11 Ready Release

A **tested, ready-to-run** build of *Need For Speed™ II Special Edition* that works out of the box on **Windows 11** (64-bit). No installation, no setup wizard, no compatibility headaches.

> ✅ **Tested and confirmed working on Windows 11 Pro (10.0.26200).**
> 🎮 **Just download the ZIP, extract, and play.**

This release is powered by the excellent cross-platform [**NFSIISE**](https://github.com/zaps166/NFSIISE) wrapper by *zaps166*, which brings the classic 1997 racer to modern systems with **hardware 3D acceleration** and **TCP/UDP network play** — bundled here as a pre-built, Windows 11-tested package.

---

## 🚀 Quick Start (Download & Play)

1. Go to the repository and download the project as a ZIP:
   **[Download ZIP](https://github.com/faai5200/NeedForSpeed2SE_Windows11/archive/refs/heads/main.zip)**
   *(Or use the green **Code → Download ZIP** button on the GitHub page.)*
2. **Extract** the ZIP to any folder (e.g. `C:\Games\NFS2SE`).
3. Double-click **`nfs2se.exe`**.
4. Start racing! 🏁

That's it — all required game data and libraries are already included.

---

## 💻 System Requirements

| | |
|---|---|
| **OS** | Windows 11 (64-bit) — *tested*. Should also run on Windows 10. |
| **Graphics** | Any GPU with OpenGL 2 support (virtually all modern cards). |
| **Disk space** | A few hundred MB after extraction. |
| **Controller** | Optional — gamepads and steering wheels are supported. |

---

## 📦 What's in the box

| File / Folder | Purpose |
|---|---|
| `nfs2se.exe` | Main game executable (OpenGL 2 renderer) — **run this**. |
| `nfs2se-gl1.exe` | Alternative executable using the OpenGL 1 renderer (for older GPUs or compatibility). |
| `SDL2.dll` | Required runtime library (already included). |
| `GAMEDATA/` | Original game data (tracks, cars, audio, etc.). |
| `FEDATA/` | Front-end data (menus, art, movies). |
| `nfs2se.conf.template` | Default configuration (copied to your profile on first run). |
| `text.*` | Localized text files (English, French, German, Italian, Spanish, Swedish). |
| `install.win` | Language / data path configuration. |
| `open_config.bat` | Opens your personal config file in Notepad. |
| `clean_config.bat` | Resets your personal configuration. |

---

## ⚙️ Configuration

On first launch, a configuration file is created at:

```
%AppData%\.nfs2se\nfs2se.conf
```

To edit it, just run **`open_config.bat`** (opens it in Notepad). Common options:

- **Fullscreen / windowed** — `StartInFullScreen` (`1` = fullscreen, `0` = window)
- **Window / render size** — `WindowSize` (e.g. `1280x960`)
- **VSync** — `VSync` (`1` = on)
- **Aspect ratio** — `KeepAspectRatio` (`1` = original 4:3)

To reset everything back to defaults, run **`clean_config.bat`**.

### Changing the language
Edit `install.win` with a plain-text editor and change the language name on the **first line** (keep the `4nn` prefix). Supported: `english`, `french`, `german`, `italian`, `spanish`, `swedish`.

---

## 🎮 In-Game Function Keys

| Key | Action | Key | Action |
|---|---|---|---|
| **F1** | Toggle rain | **F7** | Toggle mirror |
| **F2** | Car detail | **F8** | Toggle music |
| **F3** | View distance | **F9** | Toggle sound effects |
| **F4** | Toggle horizon | **F10** | Brightness |
| **F5** | Toggle HUD (player 1) | **F11** | Reset car (player 1) |
| **F6** | Toggle HUD (player 2) | **F12** | Reset car (player 2) |

---

## 🌐 Multiplayer

Network play over **TCP and UDP** is supported. Default ports are `1030` (TCP/UDP) and `1029` (host UDP), configurable in `nfs2se.conf`.
*Note: the original modem connection feature is not available.*

---

## ❓ Troubleshooting

- **Game won't start / black screen:** try running `nfs2se-gl1.exe` instead of `nfs2se.exe` (OpenGL 1 renderer).
- **Weird errors on intro movies or lockups:** set `UseOnlyOneCPU=1` in your config file.
- **Want to start fresh:** run `clean_config.bat` to reset your settings.
- **Cockpit view / night driving:** these were never part of the original 3D-accelerated version and are not available here.

---

## 📜 Credits & License

- Original game: **Need For Speed™ II Special Edition** © Electronic Arts (1997). All trademarks belong to their respective owners.
- Cross-platform wrapper: **[NFSIISE](https://github.com/zaps166/NFSIISE)** by *zaps166* — the engine that makes this run on modern systems.
- This repository packages a **pre-built, Windows 11-tested** version for easy download-and-play.

The wrapper's license applies to its source code only. This is a fan-made preservation package provided for people who own the original game. You must own *Need For Speed™ II SE* to use the included game data legally.
