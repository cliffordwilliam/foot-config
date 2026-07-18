# foot-config

My [foot](https://codeberg.org/dnkl/foot) terminal config. Deliberately minimal —
one terminal, one job; window management is left to the compositor (GNOME/Wayland).

## What's in it

- JetBrainsMono Nerd Font @ 11pt with a touch of extra line-height for breathing room
- Gruvbox dark palette
- No titlebar (`csd size=0`) — move with `Super+drag`, tile with `Super+arrows`
- Starts maximized, padding centered so leftover sub-cell pixels split evenly
- 10k lines of scrollback, beam cursor

## Install on a new machine

```sh
sudo apt install foot                      # universe repo on Ubuntu
mkdir -p ~/.config/foot
ln -s ~/repositories/foot-config/foot.ini ~/.config/foot/foot.ini
```

To make foot the default terminal on Ubuntu 25.04+ (GNOME):

```sh
echo foot.desktop > ~/.config/ubuntu-xdg-terminals.list
```

Validate the config any time with `foot --check-config` (exit 0 = OK).
Reload an open window with `Ctrl+Shift+R`.
