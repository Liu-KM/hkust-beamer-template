# hkust-beamer-template

Unofficial, community-maintained HKUST-styled Beamer template for academic presentations.

> This repository is **not** an official HKUST project. It is a community-made template inspired by HKUST presentation styling for easier slide preparation.

## Features

- 16:9 Beamer layout
- HKUST-inspired blue/gold palette
- Top navigation with section progress dots
- Single-row footer with author / title / page number
- Ready-to-edit sample deck in `slide.tex`

## Repository Layout

- `HKUST_Beamer.sty` — Beamer theme definition
- `slide.tex` — example presentation
- `pic/` — required visual assets referenced by the template
- `DISCLAIMER.md` — branding and asset usage notice

## Quick Start

Compile with XeLaTeX:

```bash
xelatex -interaction=nonstopmode slide.tex
xelatex -interaction=nonstopmode slide.tex
```

If Arial is unavailable on your machine, the template automatically falls back to `TeX Gyre Heros`.

## Customization

Edit these fields in `slide.tex`:

- `\author{...}`
- `\institute{...}`
- `\title{...}`
- `\subtitle{...}`
- `\date{...}`

Then replace the example content slides with your own material.

## Branding Notice

This repository includes HKUST-related visual assets solely to make the template usable. Those marks and logos are **not** released under the MIT license in this repository. Please read [`DISCLAIMER.md`](DISCLAIMER.md) before reusing or redistributing them.

Relevant official HKUST pages:

- Brand Assets Unit: <https://brand.hkust.edu.hk/>
- Official Marks or Logos: <https://brand.hkust.edu.hk/hkust-marks>
- University policy / guidelines entry: <https://dst.hkust.edu.hk/support-%26-resources//university-policies-%26-guidelines>

## License

The LaTeX / style code and documentation authored in this repository are released under the MIT License. HKUST marks, logos, and other official brand assets remain the property of HKUST and are excluded from that license unless HKUST explicitly states otherwise.
