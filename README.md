# Color Wheel Playground

An interactive color-harmony tool. Pick a base color, drag handles around the
wheel to explore harmonies, generate scales, and export your palette.

**Live:** https://memo-es.github.io/color-wheel/

## Features

- Interactive HSV color wheel with draggable harmony handles
- Harmony schemes: Analogous, Complementary, Split & Double Split
  Complementary, Triadic, Rectangle, Tetradic, Square, **Pentadic**
  (5 evenly-spaced mains — ideal for brand systems)
- **Real color names** fetched from the open-source [color-name-list](https://api.color.pizza)
  (api.color.pizza) — curated, unique per palette; falls back to an offline
  hue-based name if the network is unavailable. Every name is editable (click to rename)
- **Soft / Vivid variants** auto-derived per color (pale tint + saturated punch)
- **Brand-board export** — a named mosaic board in a brand-sheet layout,
  downloadable as PNG or SVG
- **Tailwind 50–950 scales** generated locally for every named color
  (uicolors-style: input color anchored at its closest shade, saturation
  curve toward the tints/shades) — with a visual preview and full
  `theme.extend.colors` config export. No API key, no network
- Optional **5th color on Tetradic** for 5-stop gradient palettes — drops a
  draggable handle into the largest hue gap (smoothest sweep), with a live
  gradient preview you can copy as a CSS `linear-gradient`
- Live readouts in Hex, RGB, HSL, HSV, and OKLCH
- Scale generator: Tailwind steps, Shades, Tints, Tones, and harmony scales
- Color picker popover (saturation/value square + hue slider) and eyedropper
- Random palette, click-to-copy swatches
- Export to CSS, SCSS, JSON, Tailwind config, SVG, hex array, or brand board
  (names and variants are carried into every code export)
- No dependencies, no build step — pure HTML/CSS/JS

## Usage

Open the live playground above, or open `index.html` directly in any modern
browser. The eyedropper requires a Chromium-based browser (Chrome/Edge).

## Project structure

- `index.html` — self-contained app

---

Ideated by [Memo Es](https://memoesparza.com) · Built with [Claude Code](https://claude.com/claude-code) help
