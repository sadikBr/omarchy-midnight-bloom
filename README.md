# Midnight Bloom

A calm dark [Omarchy](https://omarchy.org) theme: deep navy backgrounds with soft
blue, teal, lavender and peach accents. Ported from the *Midnight Bloom* Zed theme.

## Install

```bash
omarchy theme install https://gitlab.com/<your-user>/omarchy-midnight-bloom
omarchy theme set "Midnight Bloom"
```

Or manually:

```bash
cp -r omarchy-midnight-bloom ~/.config/omarchy/themes/midnight-bloom
omarchy theme set midnight-bloom
```

Omarchy generates the terminal, Hyprland, Neovim, btop, VS Code, etc. configs
from `colors.toml`.

## Extras

`extras/zed/midnight-bloom.json` is the matching Zed editor theme. Copy it to
`~/.config/zed/themes/` and pick "Midnight Bloom" in Zed.

`extras/hooks/theme-apps.sh` themes apps Omarchy doesn't cover, using the
current theme's `colors.toml`: Zen Browser (`userChrome.css`/`userContent.css` +
`user.js` in each profile) and IntelliJ IDEA (a generated "Omarchy" UI theme
plugin and editor scheme). Install it once and it re-runs on every theme change:

```bash
omarchy hook install theme-set extras/hooks/theme-apps.sh
omarchy theme set midnight-bloom
```

Restart Zen and IntelliJ afterwards; neither reloads themes while running.
