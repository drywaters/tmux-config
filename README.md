# tmux Configuration

This directory contains tmux configuration files and plugin data managed by [TPM](https://github.com/tmux-plugins/tpm).

## File locations
- `~/.config/tmux/tmux.conf` – primary tmux configuration used when tmux starts
- `~/.config/tmux/plugins/` – TPM-managed plugins installed from GitHub
- `~/.config/tmux/resurrect/` – session snapshots saved by `tmux-resurrect`

## Plugins
- `tmux-plugins/tpm` – plugin manager that installs and updates all other plugins
- `tmux-plugins/tmux-sensible` – collection of sane default settings
- `christoomey/vim-tmux-navigator` – seamless movement between Vim splits and tmux panes
- `dreamsofcode-io/catppuccin-tmux` – Catppuccin themed status bar and colours
- `tmux-plugins/tmux-yank` – augments copy mode to integrate with the system clipboard
- `tmux-plugins/tmux-open` – opens highlighted URLs or file paths from copy mode
- `tmux-plugins/tmux-resurrect` – persists sessions, windows, and panes to disk
- `tmux-plugins/tmux-continuum` – automatically saves and restores sessions on interval

## Custom configuration highlights
- Enables true colour support (`terminal-overrides`, `mouse on`)
- Changes prefix from `Ctrl-b` to `Ctrl-Space`
- Windows and panes start counting at 1 and renumber automatically
- Uses vi-style copy mode keys with custom bindings for select (`v`), rectangle toggle (`Ctrl-v`), and yank (`y`)
- Split key bindings (`"` vertical, `%` horizontal) preserve the current working directory
- `Ctrl-Shift-Left` and `Ctrl-Shift-Right` swap the current window with the previous or next
- TPM path configured to `~/.config/tmux/plugins` with TPM run command updated accordingly
- Continuum saves every 15 minutes and restores sessions on launch, storing data in `~/.config/tmux/resurrect`
