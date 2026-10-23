# MacOS Launchpad Plus

A [Windhawk](https://windhawk.net/) mod that replaces the Windows Start menu with a floating app grid inspired by the macOS Launchpad. It includes folders, pages, search, custom icons and a power menu.

![Screenshot](screenshot.png)

## Features

### Opening
- Opens with the **Windows key** and/or the **Start button** (each can be turned on or off)
- **Window** or **fullscreen** mode. Fullscreen respects the work area and the space reserved by [Standalone Dock](https://windhawk.net/)
- Opening and closing animations: **Pop**, **Fade**, **Slide** (rise from / sink into the taskbar) and **CRT**, with adjustable speed

### Search
- Shown as a **top bar** or a **centered macOS-style box**
- Also finds **apps inside folders**
- Just start typing. Supports Backspace, Ctrl+Backspace (delete a word) and Ctrl+V (paste)

### Navigation
- **Vertical scrolling** or **horizontal pages**
- Page indicators (clickable dots), mouse wheel, horizontal wheel and **swipe**
- Dragging an icon to the edge of the screen flips to the next or previous page
- Full keyboard navigation

### Folders
- Saved between sessions, with open and close animations
- Create a folder by **dragging an app onto another app**, or from the context menu
- **Drag apps into folders**; drag an app **out of an open folder** to remove it
- **Rename** a folder by clicking its title, and **Undo folder** to ungroup its apps
- Blur behind the open folder
- Apps you uninstall are removed from folders automatically

### Selection
- **Multi-select** with Ctrl+click or the context menu
- Select all, clear the selection, and drag several apps at once (a counter badge shows how many)
- Create a folder from the selected apps

### Taskbar
- **Pin to taskbar** from the context menu or by **dragging an icon onto the taskbar** (also works with the Standalone Dock)
- Pin several selected apps at once

### Custom icons
- Set a custom icon for any app: **PNG, JPG, JPEG, BMP, ICO, GIF, WebP**
- Custom icons are saved and can be reset at any time

### Power menu
- Optional power button **left or right** of the search bar
- **Lock, Sleep, Restart, Shut down, Sign out**

### Appearance
- **Blur Mode**: Adjustable (blurred snapshot of the desktop) or None
- Background color and opacity
- Border width, color and opacity
- Rounded corners for the window and for the open folder
- Icon size and number of columns

## Installation

1. Install [Windhawk](https://windhawk.net/).
2. Open Windhawk and click **Create a new mod**.
3. Replace the code with the contents of [`macos-launchpad-plus.wh.cpp`](macos-launchpad-plus.wh.cpp).
4. Click **Compile Mod**, then **Enable**.

## Controls

| Action | Shortcut |
|---|---|
| Search | Start typing |
| Delete character / word | `Backspace` / `Ctrl+Backspace` |
| Paste | `Ctrl+V` |
| Navigate / launch | Arrow keys + `Enter` |
| Scroll / change page | `Page Up` / `Page Down`, mouse wheel, swipe |
| Multi-select | `Ctrl+click` |
| Back / close | `Esc` (closes the menu, then the selection, the search, the open folder and finally the Launchpad) |

- Clicking empty space clears the selection, or closes the Launchpad if nothing is selected
- Clicking outside an open folder closes the folder
- The Launchpad closes when it loses focus

## Context menus

| Right-click on | Options |
|---|---|
| **App** | Select/Deselect, New folder with this app (or with the selection), Pin to taskbar, Change icon, Reset icon |
| **App found inside a folder (search)** | Pin to taskbar, Change icon, Reset icon |
| **Folder** | Rename, Undo folder |
| **Empty space** | New folder, Select all, Clear selection |
| **Inside an open folder** | Change/Reset icon of the app, Rename, Undo folder |

## Settings

| Setting | Default | Options / Range |
|---|---|---|
| Blur Mode | Adjustable | Adjustable, None |
| Blur strength | 60 | 0–100 (Adjustable mode only) |
| Background opacity | 60% | 0–100 |
| Background color | `#1e1e1e` | Hex color |
| Display mode | Window | Window, Fullscreen |
| Window width | 80% | 30–100 (window mode only) |
| Window height | 75% | 30–100 (window mode only) |
| Search style | Top bar | Top bar, Centered box (macOS) |
| Window corner radius | 28 px | 0–60 |
| Open folder corner radius | 26 px | 0–60 |
| Folder blur | 40 | 0–100 |
| Animation speed | 100% | 25–400 |
| Border width | 1 px | 0–8 (0 = none) |
| Border color | `#ffffff` | Hex color |
| Border opacity | 18% | 0–100 |
| Icon size | 64 px | 24–192 |
| Columns | 0 (auto) | 0–30 |
| Page navigation | Vertical | Vertical (scroll), Horizontal (pages) |
| Drag icon to taskbar to pin | On | On / Off |
| Opening animation | Pop in | Pop in, Fade, Rise from taskbar, CRT |
| Closing animation | Pop out | Pop out, Fade, Sink into taskbar, CRT |
| Open with Windows key | On | On / Off |
| Open with Start button | On | On / Off |
| Show power button | On | On / Off |
| Power button position | Left | Left, Right of the search bar |

## Notes and limitations

- The blur is a static snapshot taken when the Launchpad opens
- Search is case-insensitive substring matching. Accents are not ignored, and results are sorted alphabetically
- Apps found inside folders through search can be launched, pinned and given a new icon, but not selected or regrouped
- Power actions run without confirmation
- Pinning uses the shell `taskbarpin` verb and may fail silently if Windows doesn't offer it for an app
- Changing settings closes the Launchpad if it is open

## Changelog

### 1.2.0
- Search now includes apps inside folders
- "Blur type" renamed to "Blur Mode"; only Adjustable and None remain (Acrylic and Windows blur removed)
- Fixed credits (original mod: Fullscreen Start (Launchpad style))

### 1.1.0
- New setting: power button position (left or right of the search bar)

### 1.0.0
- First release, based on Rafael Mendes' Fullscreen Start (Launchpad style)
- Custom icons per app
- Optional power menu button

## Credits

Based on the original **Fullscreen Start (Launchpad style)** mod (`fullscreen-start`) by **Rafael Mendes** ([@RafaelMendes1407](https://github.com/RafaelMendes1407)). All credit for the original concept and implementation goes to him.

Maintained by **Thiago Silva** ([@brideinflame-rgb](https://github.com/brideinflame-rgb)).

## License

[MIT](LICENSE)
