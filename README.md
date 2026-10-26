# Siri Plus Launchpad

A [Windhawk](https://windhawk.net) mod that replaces the Windows 11 Start menu with a macOS-inspired launcher: a Siri-style search bar with a categories menu, app tabs, file search, clipboard history, quick actions and live liquid-glass effects.

Press the **Windows key** (or click **Start**) and type, or pick what you want to search from the menu that drops down from the bar.

![Original Siri mode](screenshots/Modo%20siri%20Original%20degrad%C3%AA.gif)

---

## Highlights

- **Four modes**: Original Siri (default), Floating, Window and Fullscreen
- **Live liquid glass**: real-time blur behind the bar and panels (animated wallpapers and videos keep playing underneath)
- **One search for everything**: Apps, Files, Clipboard and Actions
- **App tabs**: All, automatic categories and up to 6 tabs of your own
- **Recent apps row**: recently opened or installed apps (or the most used ones) on top
- **Power options**: type *shut down*, *restart*, *sleep*, *lock* or *sign out*, or use the floating power button
- **Custom icons**: give any app your own icon (PNG, JPG, ICO, WebP...)
- **Themes**: Clear glass, Light, Siri (macOS 27 gradient) and a fully Custom theme
- **Your language**: the interface follows the Windows display language (English, Portuguese, Spanish, French, German and Italian)

---

## Screenshots

### Original Siri (default)
| Siri | Clear glass | Light |
|---|---|---|
| <img src="screenshots/Modo%20siri%20Original%20degrad%C3%AA.gif" alt="Original Siri, Siri theme" width="100%"> | <img src="screenshots/Modo%20siri%20Original%20vidro.gif" alt="Original Siri, Clear glass theme" width="100%"> | <img src="screenshots/Modo%20siri%20Original%20Claro%20.gif" alt="Original Siri, Light theme" width="100%"> |

### Floating
| Siri | Clear glass | Light |
|---|---|---|
| <img src="screenshots/Modo%20flutuante%20degrad%C3%AA.gif" alt="Floating, Siri theme" width="100%"> | <img src="screenshots/Modo%20flutuante%20transparente.gif" alt="Floating, Clear glass theme" width="100%"> | <img src="screenshots/Modo%20flutuante%20claro.gif" alt="Floating, Light theme" width="100%"> |

### Window
![Window mode, Siri theme](screenshots/Modo%20Janela%20degrad%C3%AA.gif)

| | Siri | Clear glass | Light |
|---|---|---|---|
| Centered search box | <img src="screenshots/Modo%20janela%20degrade.png" alt="Window, Siri theme" width="100%"> | <img src="screenshots/Modo%20janela%20vidro.png" alt="Window, Clear glass theme" width="100%"> | <img src="screenshots/Modo%20janela%20claro.png" alt="Window, Light theme" width="100%"> |
| Search on the top bar | <img src="screenshots/Modo%20janela%20degrade%20pesquisa%20na%20barra%20superior.png" alt="Window, Siri theme, top bar" width="100%"> | <img src="screenshots/Modo%20janela%20vidro%20pesquisa%20na%20barra%20superior.png" alt="Window, Clear glass theme, top bar" width="100%"> | <img src="screenshots/Modo%20janela%20claro%20pesquisa%20na%20barra%20superior.png" alt="Window, Light theme, top bar" width="100%"> |

### Fullscreen
| Siri | Clear glass | Light |
|---|---|---|
| <img src="screenshots/modo%20tela%20cheia%20degrade.png" alt="Fullscreen, Siri theme" width="100%"> | <img src="screenshots/modo%20tela%20cheia%20vidro.png" alt="Fullscreen, Clear glass theme" width="100%"> | <img src="screenshots/modo%20tela%20cheia%20claro.png" alt="Fullscreen, Light theme" width="100%"> |

---

## Modes

### Original Siri (default)
A search bar in the macOS 27 style.

- **Categories menu**: hover over the bar (or click it) and a menu drops down with **Applications**, **Files**, **Actions** and **Clipboard**, each with its icon and its keyboard shortcut (default **Ctrl+1 … Ctrl+4**, configurable).
- Picking a category makes its icon and name glide from the menu into the bar, and the search then works inside that category. If you type straight away, you go to Applications.
- **Going back**: hover the category icon in the bar and it turns into a back arrow. Click it, or press **Esc**, to return to "Search" with the magnifier and pick another category.
- **App tabs**:
  - **All** comes first and shows every app.
  - Then the automatic categories: Utilities, Productivity, Entertainment, Social, Creativity, Reading and Other.
  - Then up to **6 tabs of your own**, for example "Games".
- **First row**: recently opened or installed apps, or the most used ones (configurable), separated from the rest by a thin line.
- **Actions**: Lock, Sleep, Restart, Shut down, Sign out, Settings, Task Manager, File Explorer, Control Panel, Screenshot and Empty Recycle Bin. Shut down works like Windows' own (fast startup when it is on) and warns before signing off other users who are still signed in.

### Floating
The bar appears out of an animated circle, the **Siri wave** or a soft glow, with zoom and an adjustable bounce. Clicking it or typing slides the results panel down. When it closes, the bar is "sucked" back into the bubble.

### Window and Fullscreen
The classic Launchpad grid with pages or vertical scrolling, folders and a power button. Pages always slide inside the glass. Fullscreen respects the work area and the space reserved by docks.

---

## Managing app tabs (Original Siri)

| What | How |
|---|---|
| Create a tab | Right-click an app → **New tab with this app**, or right-click the tab strip / an empty area → **New tab**. Type the name and press **Enter** |
| Add apps | Inside a tab, right-click → **Add app**. A picker shows every app: **long-press** the first one, then a simple click selects or deselects the others (selected apps jiggle); **Done** saves |
| Remove an app | Inside a tab, right-click the app → **Remove from tab** |
| Rename or delete | Right-click the tab → **Rename tab** / **Delete tab** |
| Built-in tabs | They can also be edited (add or remove apps) and deleted. **Restore default tabs** brings them back |
| Move through tabs | **Tab / Shift+Tab**, or click and drag the strip sideways (the mouse wheel works too) |

---

## Files
- **Indexer**: Everything (through IPC, no DLL needed), Windows Search or a direct scan. The default, Automatic, uses the first one that is available.
- When the search is empty, your **recent searches** are shown, with a button to clear them. History can be turned off.
- Results show the **folder** of each file under its name, in a list or as icons.
- The maximum number of results is configurable.

## Clipboard
- Keeps the texts you copy while the mod runs (in memory only, never saved). The number of items is configurable.
- **Passwords stay out**: items that password managers and browsers mark as secret are skipped, just like Windows' own clipboard history (Win+V).
- Shown as a **list**: the first line of each text, with a preview of the rest (or its size) underneath.
- Click an item to copy it again. Turning the category off also stops monitoring and clears the history.

## Apps and icons
- **Search** apps by typing.
- **Folders** (Window and Fullscreen): drag apps together, rename, undo. The Siri modes list the apps of every folder together.
- **Multi-select** with jiggling icons, **pin to taskbar** (also by dragging an icon to the taskbar), **uninstall**.
- **Custom icons**: right-click an app → **Change icon...** and pick an image (PNG, JPG, JPEG, BMP, ICO, GIF or WebP). The new icon is remembered across restarts; **Reset icon** brings back the original. Works in every mode, including apps inside folders.
- Icon size, number of columns and the scrolling direction are configurable.

---

## Customization

All options are in the mod's **Settings** tab in Windhawk, with names in English and Portuguese.

| Block | Options |
|---|---|
| ① Mode | Original Siri (default), Floating, Window, Fullscreen |
| ② Theme | Clear glass, Light, Siri (macOS 27 gradient), Custom |
| ③ Appearance | Glass transparency, corner rounding, background blur (0 = no blur) |
| ④ Custom theme | Color, opacity, dark-to-light gradient, border width, color and opacity |
| ⑤ Window and Fullscreen | Window size, search style (top bar or centered box), power button and its position, opening and closing animations (pop, fade, rise from/sink into the taskbar, CRT), animation speed, blur behind open folders |
| ⑥ Floating and Original Siri | Bar size, results box width and rows, circle animation (Siri wave, soft glow, none), circle zoom, bounce of the circle and of the results box, opening/closing duration, animation speed, power options when typing, floating power button, first row (recent, most used, off), Original Siri category shortcuts for Applications, Files, Actions and Clipboard (defaults **Ctrl+1**, **Ctrl+2**, **Ctrl+3**, **Ctrl+4**; any combination starting with Ctrl, e.g. Ctrl+Shift+F or Ctrl+F2) |
| ⑦ Opening | Open with the Windows key and/or the Start button |
| ⑧ Apps and icons | Icon size, columns, scrolling direction, jiggle, drag to the taskbar to pin |
| ⑨ Files | On/off, search history, list or icons, indexer, maximum results |
| ⑩ Clipboard | On/off, number of items kept |

---

## Keyboard and mouse

| Key / action | What it does |
|---|---|
| **Win** / Start button | Open or close |
| Type | Search (in Original Siri, typing right away searches Applications) |
| **Ctrl+1 / 2 / 3 / 4** | Original Siri: go to Applications / Files / Actions / Clipboard (configurable) |
| **Tab / Shift+Tab** | Original Siri: next/previous app tab, or move through the results in Files, Clipboard and Actions |
| Arrows + **Enter** | Move through results / open |
| Other **Ctrl+digits** | Launch the matching result (never an action such as Shut down) |
| **Esc** | Closes menus, then clears the search, goes back to the categories and finally closes |
| Right-click on the search bar | Cut, Copy, Paste, Select all, Delete all |
| Long-press an app | Select it; then a simple click selects or deselects more apps (Window/Fullscreen: right-click → **New folder with N items** puts them in a folder; Original Siri: inside the app picker) |

---

## Requirements
- Windows 11 (x64)
- [Windhawk](https://windhawk.net)
- Live blur needs **Transparency effects** turned on in Windows (*Settings → Personalization → Colors*). Without it, a blurred still image is used.
- Optional: [Everything](https://www.voidtools.com) for instant file search (run it normally, not as administrator)

## Compatibility
- **Fullscreen Start** (`fullscreen-start`): don't enable both. Each one replaces the Start menu through the same hook without calling the original, so only one of them would get the Windows key.
- **Spotlight Launcher**: it adds a separate search bar on Alt+Space and leaves the Start menu alone. This mod replaces the Start menu itself (Windows key and Start button) and adds app tabs, folders, files, clipboard history and actions. Both can be used together.

## Installation
1. Install [Windhawk](https://windhawk.net).
2. Search for **Siri Plus Launchpad** in Windhawk's mod browser and click **Install**.
   Or click **Create a new mod**, paste the contents of `siri-plus-launchpad.wh.cpp` from this repository, then **Compile** and **Enable**.
3. Press the Windows key.

---

## Support the project
If you enjoy Siri Plus Launchpad, you can support its development with a Pix donation:

[![Donate with LivePix](https://img.shields.io/badge/Donate-LivePix-00C2A8?style=for-the-badge)](https://livepix.gg/kurokobr)

---

## Credits
Originally based on the **Fullscreen Start (Launchpad style)** mod (`fullscreen-start`, MIT License) by **Rafael Mendes** ([github.com/RafaelMendes1407](https://github.com/RafaelMendes1407)). The project has since been largely rewritten and extended.

Parts that still come from (or are adapted from) his code:
- **App list and icons**: enumerating the "All apps" list (programs and Store apps), loading each app's icon and trimming/centering it, skipping non-app entries, loading them on a background thread
- **Standalone Dock integration**: respecting the space the Dock reserves and keeping the Dock above the launcher
- **Fallback blur**: capturing the screen behind the launcher and blurring it (used when Windows' transparency effects are off)
- **Drawing base**: the layered window drawn with Direct2D (surface, render target and icon bitmaps)
- **Start menu interception**: the hook that opens the launcher instead of the Windows Start menu
- **Small helpers**: text lowercasing, name sorting, color parsing, timing

Everything else (Original Siri and Floating modes, live liquid glass, themes, app tabs, folders, Files, Clipboard, Actions, menus, animations, power options, shortcuts and translations) was written for this project.

Developed and maintained by **Thiago Silva** ([github.com/brideinflame-rgb](https://github.com/brideinflame-rgb)).

## License
Copyright (c) 2026 Thiago Silva. Licensed under the **GNU General Public License v3.0** (see `LICENSE`).

The parts that come from Rafael Mendes' *Fullscreen Start* are also available under their original license:

```
MIT License
Copyright (c) Rafael Mendes

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
