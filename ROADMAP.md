# Roadmap

## Done

- [x] Browse all Honolulu, Oahu, and Kaala colors with new code, name, hex, and legacy old code
- [x] Search by name, new code, old code, hex value, or color family prefix
- [x] Sort by new code, name, hue, brightness, or old code
- [x] Compound sort options — saturation → brightness, hue → brightness, family → saturation, etc.
- [x] Group by color family — 18 families ordered around the color wheel
- [x] Family toggle toolbar — horizontal chip bar to show/hide families, with All/None
- [x] Custom family ordering — Y, YR, R, RV, V, BV, B, BG, G, YG, E, WG, CG, GG, YGY, BGY, FY, Special
- [x] Set filter — toggle Honolulu, Oahu, Kaala individually (Honolulu default)
- [x] Click any swatch to copy hex to clipboard
- [x] Print preview — flow-based paged layout with mobile-responsive scaling
- [x] Print settings — page size, filled/unfilled, label position, label info toggles, shapes, spacing
- [x] Mixed shape mode — seeded random, 1-in-5 chance of animal shapes
- [x] Static print preview — no hover/click interactivity on pages
- [x] Sticky toolbars — family bar and print panel stay visible while scrolling
- [x] Pastel Cute theme — soft coral accent, lilac/mint/peach panels, rounded corners
- [x] Mobile-friendly header — ctrl-groups keep labels with their controls

## Blocked

- [ ] Product filter — filter by Ohuhu product (e.g. 24 Basic, 96 Pastel, 320 Color). PDFs collected in `products/` folder for Honolulu, Oahu, and Kaala. Blocked on reliable OCR to extract color codes from image-based PDFs. Tesseract or Google Cloud Vision recommended.

## Planned

- [ ] Blank swatch chart export — generate printable charts with empty swatch boxes to color in
- [ ] Colored swatch chart export — filled with hex colors for digital reference
- [ ] Custom groups — select and save personal subsets (e.g. your 96-marker set)
- [ ] Export to CSV / JSON
- [ ] Procreate palette export (.swatches) — ZIP containing `Swatches.json` with HSB values normalized 0–1. Max 30 colors per palette (split into multiple files for larger sets). Can be generated client-side with JSZip. Procreate 5.0+ format adds ICC profile for better compatibility.
- [ ] Force 1 Page mode — fix conflicting transforms on mobile
