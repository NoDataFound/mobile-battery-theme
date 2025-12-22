# Mobile Battery Theme

A CSS Loader theme for Steam Deck that replaces the default battery icon with an Android 16 Material You style battery indicator.

```
Android 16 Vertical:        Android 16 Horizontal:
    ╭─╮                     ╭──────────────╮
  ╭─┴─╮                     │ ████████░░░░ ├╮
  │███│                     ╰──────────────╯╯
  │███│
  │░░░│
  ╰───╯
```

## Features

- **2 Battery Orientations**: Vertical and Horizontal layouts
- **17 Fill Colors**: White, Red, Orange, Amber, Yellow, Lime, Green, Emerald, Teal, Cyan, Sky, Blue, Indigo, Violet, Purple, Magenta, Pink, Rose
- **9 Border Colors**: Separate border color customization
- **Percentage Toggle**: Show or hide battery percentage text
- **Battery Level Display**: Shows current charge with semi-transparent depleted portion
- **State Indicators**: Low battery, critical, charging, and full states with animations

## Requirements

- Steam Deck with SteamOS
- [Decky Loader](https://github.com/SteamDeckHomebrew/decky-loader) installed
- [CSS Loader](https://github.com/DeckThemes/SDH-CssLoader) plugin installed

## Installation

### From DeckThemes Store (Recommended)
1. Open Quick Access Menu (... button) in Gaming Mode
2. Navigate to Decky > CSS Loader
3. Go to the Store tab
4. Search for "Mobile Battery Theme"
5. Click Install

### Manual Install
1. Copy the `mobile-battery-theme` folder to:
   ```
   /home/deck/homebrew/themes/
   ```
2. In Gaming Mode, open Quick Access Menu
3. Navigate to Decky > CSS Loader
4. Press "Refresh" at the bottom
5. Enable "Mobile Battery Theme"

## Configuration

After enabling the theme, use the dropdown options in CSS Loader to customize:

- **Battery Style**: Choose between Vertical or Horizontal orientation
- **Fill Color**: Select from 17 color options
- **Border Color**: Customize the border independently
- **Show Percentage**: Toggle the battery percentage text

## CSS Variables

This theme uses the `--mbt-` prefix for all CSS variables:

- `--mbt-fill-color`: Battery fill color
- `--mbt-border-color`: Battery outline color
- `--mbt-tip-color`: Battery tip color
- `--mbt-transition-speed`: Animation speed
- `--mbt-pulse-duration`: Charging pulse animation duration

## File Structure

```
mobile-battery-theme/
├── theme.json              # Theme manifest
├── shared.css              # CSS variables and animations
└── styles/
    ├── android16-horizontal.css
    ├── android16-vertical.css
    ├── color-*.css         # Fill color options
    ├── border-*.css        # Border color options
    └── hide-percentage.css
```

## License

MIT License - Feel free to modify and redistribute.

## Credits

- [Decky Loader](https://decky.xyz/)
- [DeckThemes/CSS Loader](https://deckthemes.com/)
- Inspired by Android 16 Material You battery design
