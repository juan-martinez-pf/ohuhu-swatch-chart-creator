# Ohuhu Swatch Chart Creator

A single-file HTML tool for browsing, organizing, and printing swatch charts for Ohuhu alcohol markers. Built around the Honolulu 364-color set, with a data model designed to expand to Oahu and Kaala.

## Features

- **Browse all 364 Honolulu colors** with new code, name, hex, and legacy old code
- **Search** by name, new code, old code, hex value, or color family prefix
- **Sort** by new code, name, hue, brightness, or old code
- **Group by color family** — 18 families ordered around the color wheel (Y → YR → R → RV → V → BV → B → BG → G → YG → E → FY → greys), with a sticky sidebar and scroll-spy navigation
- **Grid and list views** for visual browsing vs. quick scanning
- **Click any swatch to copy its hex** to clipboard
- **Zero dependencies** — a single `.html` file, works fully offline

## Roadmap

- [ ] Blank swatch chart export — generate printable charts with empty swatch boxes to color in
- [ ] Colored swatch chart export — filled with hex colors for digital reference
- [ ] Custom groups — select and save personal subsets (e.g. your 96-marker set)
- [ ] Product filter — filter to a specific Ohuhu set (Honolulu 96, 168, 320, etc.)
- [ ] Oahu and Kaala color sets
- [ ] Sort within family by saturation and brightness levels (using the new code structure)
- [ ] Export to CSV / JSON

## Color Code System

Ohuhu’s new code format encodes three properties:

```
YG  6  10
 │  │   └─ Brightness (0–16, higher = darker)
 │  └───── Saturation level (0–9)
 └──────── Color family (letter prefix)
```

The 18 families in this set: `Y`, `YR`, `R`, `RV`, `V`, `BV`, `B`, `BG`, `G`, `YG`, `E`, `FY`, `CG`, `GG`, `BGY`, `WG`, `YGY`, plus `Special` (Colorless Blender and Black).

## Data Source

Color data sourced from the community-maintained unified spreadsheet by [MysticSparkleWings](https://mysticsparklewings.github.io/OhuhuPaletteGenerator/), cross-referenced with Ohuhu’s official [Color Codes Index](https://ohuhu.com/pages/color-codes-index). Hex values are approximate and intended for digital reference — always verify with physical swatches.

## Usage

No install required. Open `index.html` in any modern browser.

```bash
git clone https://github.com/your-username/ohuhu-swatch-chart-creator
open index.html
```

## Contributing

Color accuracy improvements, additional marker sets, and export features welcome. The color data lives in the `COLORS` array at the top of `index.html`.

## License

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) — free to use, share, and adapt, including generated charts, as long as attribution is preserved. Generated charts must retain the attribution notice included in the output.

This project is not affiliated with or endorsed by Ohuhu. Ohuhu and Honolulu are trademarks of their respective owners. Color hex values are community-sourced approximations and may not exactly match physical marker output.
