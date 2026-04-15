# 🐧 My Hyprland Configuration

This repository contains my personal Hyprland configuration, optimized for a **Fedora 43** environment on an **ASUS ZenBook**. It is designed for a seamless transition from GNOME to a tiling window manager, focusing on productivity and high-performance visuals.

## 🛠️ System Components
- **OS:** Fedora 43
- **Window Manager:** Hyprland
- **Terminal:** Kitty
- **File Manager:** Nemo
- **Browser:** Waterfox (Flatpak)
- **Status Bar:** Waybar
- **App Launcher:** Fuzzel
- **Wallpaper:** Hyprpaper
- **Lock Screen:** Hyprlock

---

## ⌨️ Keybindings Reference

The **Super** key (Windows key) is the primary modifier (`$mainMod`).

### 🚀 Core Shortcuts
| Keybind | Action |
| :--- | :--- |
| `Super + Q` | Open Terminal (**Kitty**) |
| `Super + B` | Open Browser (**Waterfox**) |
| `Super + E` | Open File Manager (**Nemo**) |
| `Super + Space` | Open App Launcher (**Fuzzel**) |
| `Super + C` | Kill/Close active window |
| `Super + M` | Exit Hyprland / Power Menu |
| `Super + L` | **Lock System** (Hyprlock) |

### 🪟 Window Management
| Keybind | Action |
| :--- | :--- |
| `Super + Arrows` | Move focus between windows |
| `Super + V` | Toggle Floating mode |
| `Super + Y` | **Pin/Sticky mode** (Keep window on all workspaces) |
| `Super + P` | Pseudo-tiling |
| `Super + J` | Toggle Split (Vertical/Horizontal) |
| `Super + Alt + Arrows` | **Resize** active window (Keyboard) |
| `Super + LMB + Drag` | Move window (Mouse) |
| `Super + RMB + Drag` | Resize window (Mouse) |

### 🧭 Workspace Navigation
| Keybind | Action |
| :--- | :--- |
| `Super + [1-0]` | Switch to Workspace 1-10 |
| `Super + Shift + [1-0]` | Move window to Workspace 1-10 |
| `Super + Ctrl + Left/Right` | Cycle workspaces |
| `Super + Mouse Scroll` | Cycle workspaces |
| `3-Finger Swipe` | Cycle workspaces (Trackpad) |
| `Super + S` | Toggle **Magic Workspace** (Scratchpad) |
| `Super + Shift + S` | Send window to Magic Workspace |

---

## 🔧 Specific Fixes & Optimizations
The configuration includes the following "Daily Driver" improvements:

* **XWayland Scaling:** `force_zero_scaling = true` is enabled to prevent blurriness in non-native Wayland apps.
* **Qt/VLC Blur Fix:** Environment variables are set to force native Wayland rendering for Qt6 apps.
* **Screen Sharing:** D-Bus environment variables are synced on launch for Discord/Vesktop support.
* **Autostart:**
    * **MEGAsync** for cloud storage.
    * **AB Download Manager** for downloads.
    * **Waybar & Hyprpaper** for UI and visuals.

---

## 📂 Configuration Locations
- **Main Config:** `~/.config/hypr/hyprland.conf`
- **Wallpaper:** `~/.config/hypr/hyprpaper.conf`
- **Lock Screen:** `~/.config/hypr/hyprlock.conf`
- **Status Bar:** `~/.config/waybar/config`
