# tmux

default prefix -> ctrl + b

custom prefix -> ctrl + space

# README: Setting up tmux with Nerd Font and TPM Plugins

## Introduction
This guide will help you set up tmux, a terminal multiplexer, with Nerd Font for enhanced symbol support and TPM (Tmux Plugin Manager) for easy plugin management.

## Prerequisites
Before proceeding, make sure you have the following installed:
- tmux
- Nerd Font (Agave)
- TPM (Tmux Plugin Manager)

## Installation

### linux installation 

#### Debian-based (e.g., Debian, Ubuntu):
```bash
sudo apt update
sudo apt install tmux
```
#### Arch Linux:
```bash
sudo pacman -Sy tmux
```
#### Fedora:
```bash

sudo dnf install tmux
```
### Nerd Font Setup
1. Install Nerd Font (Agave) on your system.
2. Set Nerd Font (Agave) as your default font in your terminal emulator.

### TPM Installation
1. Clone TPM repository:
   ```bash
   git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
   ```

### Executing Configuration
1. After editing `~/.tmux.conf`, execute the configuration changes:
   ```bash
   tmux source ~/.tmux.conf
   ```

## TPM Plugins

### List of Plugins
- [tmux-plugins/tpm](https://github.com/tmux-plugins/tpm)
- [2kabhishek/tmux2k](https://github.com/2kabhishek/tmux2k)
- [tmux-plugins/tmux-sensible](https://github.com/tmux-plugins/tmux-sensible)
- [tmux-plugins/tmux-sidebar](https://github.com/tmux-plugins/tmux-sidebar)
- [jaclu/tmux-menus](https://github.com/jaclu/tmux-menus)
- [tmux-plugins/tmux-open](https://github.com/tmux-plugins/tmux-open)
- [tmux-plugins/tmux-copycat](https://github.com/tmux-plugins/tmux-copycat)
- [tmux-plugins/tmux-yank](https://github.com/tmux-plugins/tmux-yank)
- [charlietag/tmux-split-statusbar](https://github.com/charlietag/tmux-split-statusbar)
- [schasse/tmux-jump](https://github.com/schasse/tmux-jump)
- [tmux-plugins/tmux-resurrect](https://github.com/tmux-plugins/tmux-resurrect)
- [tmux-plugins/tmux-continuum](https://github.com/tmux-plugins/tmux-continuum)

  
### Installing Plugins
1. Add the desired plugin to `~/.tmux.conf` with:
   ```bash
   set -g @plugin 'tmux-plugins/tmux-sensible'
   ```
   
2. Press `prefix` + `I` to fetch and install the plugin.

### Uninstalling Plugins
1. Remove or comment out the plugin from `~/.tmux.conf`.
2. Press `prefix` + `alt` + `u` to remove/uninstall the plugin.

## Key Bindings
- `prefix` + `I`: Installs new plugins from any other repository and refreshes TMUX environment.
- `prefix` + `U`: Updates plugin(s).
- `prefix` + `alt` + `u`: Removes/uninstalls plugins not on the plugin list.

## Conclusion
You have successfully set up tmux with Nerd Font and TPM plugins. Enjoy the enhanced terminal multiplexing experience!


