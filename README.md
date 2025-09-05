# Neovide Configuration

This repository contains my personal [Neovide](https://neovide.dev/) configuration files. Neovide is a simple, no-nonsense, cross-platform graphical user interface for [Neovim](https://neovim.io/).

## About Neovide

Neovide provides a modern GUI experience for Neovim while maintaining the familiar terminal-like functionality. It offers graphical improvements and smooth animations without compromising the core Neovim experience.

- **Website**: [https://neovide.dev/](https://neovide.dev/)
- **GitHub Repository**: [https://github.com/neovide/neovide](https://github.com/neovide/neovide)

## Configuration Overview

The main configuration is stored in `config.toml` and includes the following customizations:

### Window & Display Settings
- **Fork Process**: `fork = true` - Runs Neovide as a background process
- **Frame Style**: `frame = "buttonless"` - Clean, minimalist window frame
- **Color Profile**: `srgb = true` - Uses sRGB color space for accurate colors
- **VSync**: `vsync = true` - Prevents screen tearing
- **Title Bar**: `title-hidden = true` - Hides the window title bar for cleaner look
- **Tabs**: `tabs = false` - Disables tab bar (using Neovim's native buffer management)

### Font Configuration
- **Font Family**: `ComicCodeLigatures Nerd Font` (custom patched)
- **Font Size**: `15.0`

This font choice provides:
- Programming ligatures for better code readability
- Nerd Font icons (manually patched)
- Comic Sans-inspired design that's surprisingly readable for code
- Optimized for coding with good character distinction

### Box Drawing
- **Mode**: `font-glyph` - Uses font glyphs for drawing boxes and borders
- **Default Size**: `[2, 10]` - Custom sizing for box drawing elements

## Installation

1. Make sure you have Neovide installed on your system
2. Clone or copy this configuration to your Neovide config directory:
   - **macOS/Linux**: `~/.config/neovide/`
   - **Windows**: `%APPDATA%\neovide\`

## Font Requirements

This configuration uses `ComicCodeLigatures Nerd Font`, which is a custom patched version of the paid ComicCode font. You have two options:

### Option 1: Use ComicCode (Paid Font)
1. **Purchase ComicCode** from [https://tosche.net/fonts/comic-code](https://tosche.net/fonts/comic-code)
2. **Patch it with Nerd Font icons** using the [Nerd Font patcher](https://github.com/ryanoasis/nerd-fonts#font-patcher)
3. Install the patched font on your system

### Option 2: Use Alternative Nerd Fonts (Free)
Choose any font from [Nerd Fonts](https://www.nerdfonts.com/) and modify the config:

1. Download a font like:
   - `JetBrainsMono Nerd Font`
   - `FiraCode Nerd Font` 
   - `CascadiaCode Nerd Font`
   - `Hack Nerd Font`
2. Install the font on your system
3. Update `config.toml`:
   ```toml
   [font]
   normal = "Your Chosen Nerd Font"
   size = 15.0
   ```

## Usage

Simply launch Neovide after placing the configuration file in the correct location. The settings will be automatically applied.

```bash
neovide
```

## Customization

Feel free to modify `config.toml` to suit your preferences. For a complete list of available configuration options, check the [official Neovide documentation](https://neovide.dev/configuration.html).

### Common Customizations

- Change font: Modify `font.normal` and `font.size`
- Enable tabs: Set `tabs = true`
- Show title: Set `title-hidden = false`
- Different frame style: Change `frame` to `"full"`, `"none"`, or `"transparent"`

## Contributing

This is a personal configuration, but feel free to use it as a starting point for your own Neovide setup. If you have suggestions or improvements, please open an issue or pull request.

## License

This configuration is provided as-is for personal use. Feel free to modify and distribute as needed.

---

*For more information about Neovide, visit the [official website](https://neovide.dev/) or check out the [GitHub repository](https://github.com/neovide/neovide).*
