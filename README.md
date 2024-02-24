# tmux

# prefix -> ctrl + space

# README: Setting up tmux with Nerd Font and TPM Plugins



## Introduction
This guide will help you set up tmux, a terminal multiplexer, with Nerd Font for enhanced symbol support and TPM (Tmux Plugin Manager) for easy plugin management.

## Prerequisites
Before proceeding, make sure you have the following installed:
- tmux
- Nerd Font (Agave)
- TPM (Tmux Plugin Manager)

## Installation

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
   ``

## TPM Plugins

### List of Plugins
- `tmux-sensible`: A set of sensible defaults for tmux.
  
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
```

