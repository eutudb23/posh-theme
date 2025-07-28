# iTerm2 10K Oh My Posh Theme

A modern, clean PowerShell theme inspired by the popular iTerm2 10K theme, designed for use with [Oh My Posh](https://ohmyposh.dev/).

## ✨ Features

- **Clean Design**: Minimalist aesthetic with a focus on readability
- **OS Detection**: Automatically displays your operating system with appropriate icons
- **Path Display**: Shows current directory path with folder icons
- **Git Integration**: Displays current git branch and status
- **Time Display**: Shows current time in the right prompt
- **Powerline Symbols**: Uses powerline symbols for smooth segment transitions
- **Color Scheme**: Dark theme with carefully chosen colors for optimal contrast

## 🎨 Theme Preview

The theme includes:
- **Left Prompt**: OS icon, current path, and git status
- **Right Prompt**: Current time
- **iterm2 with p10k**: as close as possible to iterm2 p10k theme

## 📋 Prerequisites

Before using this theme, ensure you have:

1. **PowerShell 7+** installed
2. **Oh My Posh** installed
3. **A Nerd Font** installed (recommended: [CaskaydiaCove Nerd Font](https://github.com/ryanoasis/nerd-fonts/tree/master/patched-fonts/CascadiaCode))

### Installing Oh My Posh

```powershell
# Install Oh My Posh
winget install JanDeDobbeleer.OhMyPosh -s winget

# Or using PowerShell
Install-Module oh-my-posh -Scope CurrentUser
```

### Installing a Nerd Font

1. Download a Nerd Font from [nerdfonts.com](https://www.nerdfonts.com/)
2. Install the font on your system
3. Configure your terminal to use the Nerd Font

## 🚀 Installation

1. **Clone or download** this repository
2. **Copy** the `iterm210k.omp.json` file to your desired location
3. **Configure** Oh My Posh to use this theme

### Configuration

Add the following to your PowerShell profile (`$PROFILE`):

```powershell
# Load Oh My Posh theme
oh-my-posh init pwsh --config "path\to\iterm210k.omp.json" | Invoke-Expression
```

To find your PowerShell profile location:
```powershell
echo $PROFILE
```

To create/edit your profile:
```powershell
notepad $PROFILE
```

## 🎛️ Customization

The theme is highly customizable. You can modify the `iterm210k.omp.json` file to:

### Change Colors
- Modify `background` and `foreground` properties in each segment
- Current color scheme uses dark backgrounds with bright foregrounds

### Modify Icons
- Update OS icons in the `properties` section
- Change folder icons and separators
- Customize git status symbols

### Adjust Layout
- Change segment order
- Modify spacing and alignment
- Add or remove segments

### Example Customizations

```json
{
  "background": "#your-color",
  "foreground": "#your-color",
  "properties": {
    "time_format": "HH:mm:ss"
  }
}
```

## 📁 File Structure

```
posh-theme/
├── iterm2p10k.omp.json    # Main theme configuration
└── README.md             # This file
```

## 🔧 Troubleshooting

### Font Issues
If icons appear as boxes or question marks:
1. Ensure you're using a Nerd Font
2. Restart your terminal after font installation
3. Verify font configuration in your terminal settings

### Theme Not Loading
1. Check the path to your theme file
2. Verify Oh My Posh is properly installed
3. Ensure your PowerShell profile is being loaded

### Performance Issues
- The theme is optimized for performance
- If you experience slowdowns, consider reducing the number of segments

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features
- Submit pull requests
- Improve documentation

## 📄 License

This theme is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- Inspired by the [iTerm2 10K theme](https://github.com/romkatv/powerlevel10k)
- Built with [Oh My Posh](https://ohmyposh.dev/)
- Uses [Nerd Fonts](https://www.nerdfonts.com/) for icons

## 📞 Support

If you encounter any issues or have questions:
1. Check the [Oh My Posh documentation](https://ohmyposh.dev/docs/)
2. Search existing issues in this repository
3. Create a new issue with detailed information

---

**Enjoy your new PowerShell experience! 🎉** 