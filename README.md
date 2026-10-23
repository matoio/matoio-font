<picture>
  <source media="(prefers-color-scheme: dark)" srcset="matoio-logo-dark.svg">
  <img src="matoio-logo.svg" alt="matoio" width="320">
</picture>

**English** · [简体中文](README.zh-CN.md)

# matoio

A rounded geometric display typeface, grown from the matoio wordmark. Version 1.000.
**Free for personal use · commercial use requires a license from [matoio.com](https://matoio.com).**

![matoio typeface preview](images/preview.svg)

- **Live demo**: https://matoio.github.io/matoio-font/
- **Design**: by mato io
- **Website**: https://matoio.com
- **Contact**: admin@matoio.com

## License

- **Personal, non-commercial use: free.** Study, practice and hobby projects that earn no income.
- **Commercial use: paid license required.** Anything for a company or client, work that earns income, websites, apps and logos counts as commercial. Licenses and prices: **https://matoio.com**.
- **Not allowed**: selling or redistributing the font files, re-releasing the font renamed or modified, or making marks that look like the matoio logo.
- Full terms in [`LICENSE`](LICENSE). Not sure whether your use needs a license? Email admin@matoio.com first.

## Files

| File | Use |
|---|---|
| `matoio-Regular.otf` | Desktop install (recommended; most precise curves in design apps) |
| `matoio-Regular.ttf` | Desktop install (widest compatibility, including older apps) |
| `matoio-Regular.woff2` | Web use (smallest, about 6.5 KB; web use needs a web license) |
| `features.fea` | OpenType feature source (kerning, figure switching), for future edits |
| `LICENSE` | License notice (English and Chinese): free for personal use, paid for commercial use |
| `index.html` | Live demo page, set in `matoio-Regular.woff2` (served by GitHub Pages) |
| `images/preview.svg`, `images/preview.png` | Preview images for this README and link cards |
| `matoio-logo.svg`, `matoio-logo-dark.svg` | matoio logo (the dark version has a white "io") |

## Live demo (GitHub Pages)

`index.html` is published with GitHub Pages at **https://matoio.github.io/matoio-font/** (source: root of the `main` branch). Every line on the page is live text in `matoio-Regular.woff2`, and there is a type tester to try your own words.

## Install

- **Windows**: right-click the `.otf` or `.ttf` → **Install** (or "Install for all users").
- **macOS**: double-click the `.otf` → **Install** in Font Book.
- Then pick **matoio** from your app's font list.

## Web use

```css
@font-face {
  font-family: "matoio";
  src: url("matoio-Regular.woff2") format("woff2");
  font-display: swap;
}
body { font-family: "matoio", system-ui, sans-serif; }
```

Characters the font does not include (Chinese, €, @, # …) fall back to `system-ui, sans-serif`.

## Character set

- **Letters**: a–z, A–Z (52).
- **Figures**: 0–9, tabular by default, plus a proportional set.
- **Punctuation**: `. , : ; ! ? ' " ‘ ’ “ ” - – — ( ) / &`.
- **Symbols**: `% ¥ $`.
- **Spaces**: space and no-break space.
- **Not included**: Chinese, other currency signs (€ £) and symbols such as @ # * + =. These are shown in the system's default font.

The punctuation is drawn in a flat-cut wedge style: commas and quotes are slanted trapezoids with straight cuts, dashes are rectangles, and the dots match the dot on the i. It follows the quiet, crisp look of ordinary system-font punctuation, and was drawn from scratch with trapezoids, rectangles, arcs and straight lines, without tracing or extracting outlines from any existing font.

## OpenType features

| Feature | What it does | Default | CSS |
|---|---|---|---|
| `kern` kerning | 181 pairs tightened automatically: 149 letter pairs (e.g. Ty, AV, To) and 32 punctuation pairs (e.g. T., Y,, L’, “A) | on | `font-kerning: normal;` |
| `tnum` tabular figures | Every figure is the same width, so prices and tables line up | on | `font-variant-numeric: tabular-nums;` |
| `pnum` proportional figures | Figures take their natural widths, for posters and headlines | off | `font-variant-numeric: proportional-nums;` |

In Figma, Illustrator, InDesign and similar apps, proportional figures are in the "OpenType" or "Figures" panel.

## Specs

- 1000 units per em.
- Cap height 694, x-height 528.
- Ascender 714, descender −186.
- Stroke weight 156 (the design's 78 at 2× scale).
- Vertical metrics: ascent 760, descent −240, line gap 0, so the default line height is about 1.0 em. For running text, set line-height to 1.2–1.3.

## Known limitations

- **Character set**: Latin letters, figures and common punctuation only; other characters fall back to a system font. In the few apps that show missing characters as boxes, switch those characters to another font by hand.
- **Weights**: a single weight (Regular, visually bold).
