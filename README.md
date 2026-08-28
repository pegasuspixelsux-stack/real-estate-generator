# Estate Studio — Real Estate Social Graphic Designer

A single-file, zero-build tool for designing luxury real-estate social media graphics.
Open `index.html` in any modern browser — no server, no install.

## Features

- **Live preview** — split-screen: controls on the left, a true-scale canvas on the right.
- **Formats** — Portrait 4:5 (1080×1350), Square 1:1, Landscape 16:9, Story 9:16.
- **Layouts** — Centered, Left Rail, Editorial, Lower Bar, and Top & Bottom framing
  (brand header pinned to the top, all detail copy in a gradient-backed lower half).
- **Design presets** — one tap sets format, layout, type, accent colour, overlay and spec style.
- **Typography** — four curated pairings (Cinzel/Parisienne, Playfair/Dancing Script,
  Bodoni Moda/Pinyon Script, Cormorant/Sacramento) via Google Fonts.
- **Quick Import Text** — paste a block of copy and the parser maps it into fields.
  Understands labelled lines (`Header:`, `Title:`, `Price:`, `Beds:` …) in English and Spanish,
  or falls back to positional mapping (line 1 → header, 2 → title, 3 → subtitle).
- **Structured specs** — three render styles: inline text, columns, or icon grid.
- **Dark gradient overlay** — always on for text legibility, with an adjustable intensity slider
  and a per-preset colour tint.
- **High-res PNG export** — exports the canvas at 2× via
  [`html-to-image`](https://github.com/bubkoo/html-to-image); web fonts are inlined as base64 so
  the file matches the preview exactly.

## Stack

- [Tailwind CSS](https://tailwindcss.com/) (CDN)
- [html-to-image](https://github.com/bubkoo/html-to-image) (CDN)
- Google Fonts

## Development

```bash
# just open it
start index.html          # Windows
open index.html           # macOS

# or serve it (needed only for browser-automation tooling)
npx serve .
```

## `inspiration/`

Holds notes on the visual direction. The reference listing graphics that informed the built-in
presets are kept locally and git-ignored — the presets distil composition, colour and layout
ideas only, never any brand's logo or exact design.
