# 🖥️ terminal-setup-for-dev

> My macOS terminal setup inspired by [Omarchy] 
> Ported and adapted for macOS using Ghostty, Zsh, and the same tools that make Omarchy feel so clean.

---

## ✨ What it looks like

- **Theme:** Catppuccin Frappé 
- **Font:** JetBrainsMono Nerd Font Mono 
- **Prompt:** Starship — minimal, just directory + git info
- **Shell:** Zsh + Oh My Zsh + modern CLI replacements

---

## 🧰 Tools Used

### Terminal
| Tool | What it does |
|------|-------------|
| [Ghostty](https://ghostty.org) | Fast, GPU-accelerated terminal emulator |
| [Catppuccin Frappé](https://github.com/catppuccin/ghostty) | Ghostty color theme (built-in) |
| [JetBrainsMono Nerd Font](https://www.nerdfonts.com) | Terminal font with icons |

### Shell & Prompt
| Tool | What it does |
|------|-------------|
| [Zsh](https://zsh.org) | Shell (default on macOS) |
| [Oh My Zsh](https://ohmyz.sh) | Zsh framework & plugin manager |
| [Starship](https://starship.rs) | Minimal, fast cross-shell prompt |

### Zsh Plugins
| Plugin | What it does |
|--------|-------------|
| [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions) | Fish-like command suggestions |
| [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting) | Syntax coloring as you type |

### Modern CLI Replacements (Omarchy-inspired)
| Tool | Replaces | What it does |
|------|----------|-------------|
| [eza](https://github.com/eza-community/eza) | `ls` | Better file listing with icons & git info |
| [bat](https://github.com/sharkdp/bat) | `cat` | Syntax-highlighted file viewer |
| [ripgrep](https://github.com/BurntSushi/ripgrep) | `grep` | Blazing fast search |
| [fd](https://github.com/sharkdp/fd) | `find` | Simple, fast file finder |
| [zoxide](https://github.com/ajeetdsouza/zoxide) | `cd` | Smarter directory jumping |
| [fzf](https://github.com/junegunn/fzf) | — | Fuzzy finder for files, history & more |

---

## 🚀 Installation

### 1. Install Ghostty
Download from [ghostty.org](https://ghostty.org) or:
```bash
brew install --cask ghostty
```

### 2. Install the font
```bash
brew install --cask font-jetbrains-mono-nerd-font
```

### 3. Copy Ghostty config
```bash
mkdir -p ~/.config/ghostty
cp ghostty/config ~/.config/ghostty/config
```

### 4. Install Oh My Zsh
```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

### 5. Install Zsh plugins
```bash
brew install zsh-autosuggestions zsh-syntax-highlighting
```

### 6. Install Starship
```bash
brew install starship
mkdir -p ~/.config
cp starship/starship.toml ~/.config/starship.toml
```

### 7. Install modern CLI tools
```bash
brew install eza bat ripgrep fd zoxide fzf
```

### 8. Apply Zsh config
```bash
cp zsh/.zshrc ~/.zshrc
source ~/.zshrc
```

---

## 📁 Repo Structure

```
terminal-setup-for-dev/
├── ghostty/
│   └── config           # Ghostty terminal config
├── zsh/
│   └── .zshrc           # Zsh shell config
├── starship/
│   └── starship.toml    # Starship prompt config
└── README.md
```

---

## 📝 License

MIT — do whatever you want with it.
