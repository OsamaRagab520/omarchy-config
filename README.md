# Omarchy Config

My customizations for [Omarchy](https://omarchy.org/) Linux.

## Hyprland

### Monitor Setup (`hypr/monitors.conf`)
- Three monitor setup:
  - **Left**: BenQ GW2480 (1920x1080) on HDMI-A-1
  - **Center (main)**: Samsung Odyssey G5 (2560x1440@165Hz) on DP-3
  - **Right (portrait)**: Dell P2219H (1920x1080, rotated 270°) on DP-1

### Workspace Bindings (`hypr/hyprland.conf`)
- Workspaces 1-3: Left monitor
- Workspaces 4-6: Center monitor
- Workspaces 7-9: Right monitor

### Keybindings (`hypr/bindings.conf`)
Vim-style navigation:
- `Super + H/J/K/L`: Move focus left/down/up/right
- `Super + Ctrl + J/K`: Next/previous workspace
- `Super + Ctrl + H/L`: Move window to left/right group
- `Super + Shift + H/J/K/L`: Swap window in direction
- `Super + Ctrl + Shift + J/K`: Move window to next/previous workspace
- `Super + Ctrl + Shift + H/L`: Move window to left/right monitor
- `Super + Alt + H/L`: Previous/next group tab
- `Super + Shift + S`: Screenshot to clipboard
- `Super + P`: Application launcher (Walker)
- `Super + M`: Omarchy menu
- `Super + Q`: Close window

### Input (`hypr/input.conf`)
- Keyboard layouts: US and Arabic with `Super + Space` toggle
- Ghostty scroll touchpad: 0.6

### Look & Feel (`hypr/looknfeel.conf`)
- Window rounding: 8px

## Terminal

### Alacritty (`alacritty/alacritty.toml`)
- Font: JetBrainsMono Nerd Font, size 9
- Padding: 14px
- No window decorations

### Ghostty (`ghostty/config`)
- Font: JetBrainsMono Nerd Font, size 9
- Padding: 14px
- Block cursor (no blink)
- Tab navigation: `Alt + H/L`
- Mouse scroll multiplier: 0.95

## Installation

Copy configs to `~/.config/`:

```bash
cp -r hypr/* ~/.config/hypr/
cp -r alacritty/* ~/.config/alacritty/
cp -r ghostty/* ~/.config/ghostty/
```
