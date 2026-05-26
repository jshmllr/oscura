![Preview](https://pub-44410522d40d4d4da6715f60f585b00c.r2.dev/misc/oscura-preview.jpg)

# Oscura by Fey

Fey's theme features meticulously curated accent colors and precisely balanced contrast, crafting a sophisticated coding environment that's both elegant and easy on the eyes. Available in two variants: **Midnight** for those who prefer deep contrast, and **Dusk** for a more moderate viewing experience.

## Recommended Settings and extension

For the best experience, we recommend using these settings in the cursor's settings.json:

```json
{
  "editor.fontFamily": "'SF Mono', 'Fira Code'",
  "editor.fontSize": 12,
  "editor.lineHeight": 1.6
}
```

For proper syntax highlighting of styled-components, we recommend installing the [vscode-styled-components](https://marketplace.visualstudio.com/items?itemName=styled-components.vscode-styled-components) extension.

## About

This theme is crafted by the Fey team, following our design's color palette and principles. It's part of our commitment to creating beautiful tools. [Fey.com](https://fey.com)

## Installation

### VScode Marketplace

Search for "Oscura Theme" in the VSCode extensions panel or click "Install" from the marketplace website.

<a href="https://marketplace.visualstudio.com/items?itemName=Fey.oscura"><strong>Install now</strong></a>

### Open VSX

For editors that use Open VSX Registry (VSCodium, Fleet, Windsurf etc) or require manual installation, you can download the `.vsix` file directly. After downloading, install it through your editor's extension menu using the "Install from VSIX" option.

<a href="https://open-vsx.org/extension/Fey/oscura"><strong>Install now</strong></a>

---

## Ports

This fork adds matching ports of Oscura for other tools, so you can carry the palette across your terminal and CLI agent. Both variants — **Midnight** (deeper contrast, `#0B0B0F`) and **Dusk** (softer, `#131419`) — are included. Original VSCode theme by [Fey](https://fey.com); see [narative/oscura](https://github.com/narative/oscura).

### Ghostty

Ports live at [`ghostty/oscura-midnight`](./ghostty/oscura-midnight) and [`ghostty/oscura-dusk`](./ghostty/oscura-dusk).

```bash
mkdir -p ~/.config/ghostty/themes

# Midnight
curl -fsSL https://raw.githubusercontent.com/jshmllr/oscura/main/ghostty/oscura-midnight \
  -o ~/.config/ghostty/themes/oscura-midnight

# Dusk
curl -fsSL https://raw.githubusercontent.com/jshmllr/oscura/main/ghostty/oscura-dusk \
  -o ~/.config/ghostty/themes/oscura-dusk
```

Then in `~/.config/ghostty/config` set one of:

```
theme = oscura-midnight
# or
theme = oscura-dusk
```

### Claude Code

Ports live at [`claude/oscura-midnight.json`](./claude/oscura-midnight.json) and [`claude/oscura-dusk.json`](./claude/oscura-dusk.json), using the custom-theme override schema.

```bash
mkdir -p ~/.claude/themes

# Midnight
curl -fsSL https://raw.githubusercontent.com/jshmllr/oscura/main/claude/oscura-midnight.json \
  -o ~/.claude/themes/oscura-midnight.json

# Dusk
curl -fsSL https://raw.githubusercontent.com/jshmllr/oscura/main/claude/oscura-dusk.json \
  -o ~/.claude/themes/oscura-dusk.json
```

Then in Claude Code run `/theme` and pick **Oscura Midnight** or **Oscura Dusk**.
