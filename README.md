# .dotfiles

Personal dotfiles for Bash, Git, and terminal tools.

## Requirements

### FiraCode Nerd Font

Used by the terminal and Starship prompt for icons and ligatures.

1. Download from [Nerd Fonts](https://www.nerdfonts.com/font-downloads) — search for **FiraCode Nerd Font**
2. Install the font on your system
3. Set it as the font in your terminal emulator

### Catppuccin Macchiato

Color theme used across the setup. Already configured in `starship.toml`.

To apply it to your terminal emulator, grab the theme for your app from the [official Catppuccin repo](https://github.com/catppuccin/catppuccin).
- https://github.com/catppuccin/windows-terminal

---

## Tools

The following tools are configured in `.bashrc`. Install them to get the full experience:

| Tool | Description | Install |
|---|---|---|
| [bat](https://github.com/sharkdp/bat) | Better `cat` with syntax highlighting | `apt install bat` |
| [lsd](https://github.com/lsd-rs/lsd) | Modern `ls` with icons and colors | `apt install lsd` |
| [starship](https://starship.rs) | Cross-shell prompt | `curl -sS https://starship.rs/install.sh \| sh` |
| [zoxide](https://github.com/ajeetdsouza/zoxide) | Smart `cd` replacement | `apt install zoxide` |
| [direnv](https://direnv.net) | Per-directory environment variables | `apt install direnv` |

> All tools are optional — the `.bashrc` checks if each one is installed before activating it.

---

## Setup

```bash
# Clone the repo
git clone git@github.com:GabiVega362/.dotfiles.git ~/.dotfiles

# Copy the dotfiles to your home directory
cp ~/.dotfiles/.bashrc ~/
cp ~/.dotfiles/.gitconfig ~/
cp ~/.dotfiles/.config/starship.toml ~/.config/
cp ~/.dotfiles/.curlrc ~/
cp ~/.dotfiles/.wgetrc ~/

# Reload bash
source ~/.bashrc
```

