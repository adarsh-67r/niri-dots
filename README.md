# niri-dots

My personal dotfiles for [niri](https://github.com/YaLTeR/niri) (a scrollable-tiling Wayland compositor) configured to work with [DankMaterialShell](https://github.com/dankerk/dankmaterialshell).

## ⚠️ Prerequisites

**This configuration is intended to be used AFTER installing DankMaterialShell.**

Before using these dotfiles, make sure you have:
- [DankMaterialShell](https://github.com/dankerk/dankmaterialshell) installed and working
- [niri](https://github.com/YaLTeR/niri) compositor installed
- A Wayland-compatible system

## 📦 What's Included

This repository contains:
- **niri configuration** (`niri/config.kdl`) - Main niri compositor configuration
- **DankMaterialShell settings** (`DankMaterialShell/settings.json`) - Custom DMS theme and widget settings
- **niri/dms/** - DMS-specific niri configurations:
  - `wpblur.kdl` - Wallpaper and blur settings
  - `layout.kdl` - Window layout configuration
  - `binds.kdl` - Keybindings
  - `colors.kdl` - Color scheme
  - `alttab.kdl` - Alt-tab switcher configuration

## 🚀 Installation

1. **Install DankMaterialShell first** (if you haven't already):
   ```bash
   # Follow the installation instructions at:
   # https://github.com/dankerk/dankmaterialshell
   ```

2. **Backup your existing configurations** (if any):
   ```bash
   # Backup niri config
   mv ~/.config/niri ~/.config/niri.backup
   
   # Backup DankMaterialShell settings
   mv ~/.config/DankMaterialShell ~/.config/DankMaterialShell.backup
   ```

3. **Clone and apply these dotfiles**:
   ```bash
   git clone https://github.com/adarsh-67r/niri-dots.git
   cd niri-dots
   
   # Copy niri configuration
   cp -r niri ~/.config/
   
   # Copy DankMaterialShell settings
   cp -r DankMaterialShell ~/.config/
   ```

4. **Restart niri**:
   ```bash
   niri msg action quit
   # Then log back in to niri
   ```

## 🎨 Configuration Highlights

- **Dynamic theming** with matugen color schemes
- **Custom DankMaterialShell widgets**: weather, music, clipboard, system monitor
- **Optimized for touch**: Touchpad gestures and hot corners enabled
- **24-hour clock format** with weather for Rourkela, Odisha
- **Auto-hiding dock** with circular indicators
- **Custom keybindings** tailored for niri workflow

## 📸 Screenshots

<!-- Add your screenshots here -->

### Desktop
*Screenshot placeholder - Add your desktop screenshot here*

### DankMaterialShell Bar
*Screenshot placeholder - Add your bar screenshot here*

### Niri Overview
*Screenshot placeholder - Add your overview screenshot here*

### Control Center
*Screenshot placeholder - Add your control center screenshot here*

## 🛠️ Customization

Feel free to modify the configurations to suit your preferences:

- **DankMaterialShell settings**: Edit `~/.config/DankMaterialShell/settings.json`
- **Niri keybindings**: Edit `~/.config/niri/dms/binds.kdl`
- **Colors**: Edit `~/.config/niri/dms/colors.kdl`
- **Layout**: Edit `~/.config/niri/dms/layout.kdl`

## 📝 Notes

- Weather is configured for **Rourkela, Odisha** - update coordinates in `settings.json` for your location
- Font is set to **FiraCode Nerd Font** - install it or change to your preferred font
- Display output is configured for **eDP-2** - adjust for your monitor setup

## 🙏 Credits

- [niri](https://github.com/YaLTeR/niri) by YaLTeR
- [DankMaterialShell](https://github.com/dankerk/dankmaterialshell) by dankerk

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.