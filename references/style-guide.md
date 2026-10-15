# Black-background visual style

## Identity

- Canvas: `#000000`. Primary text: `#FFFFFF`. Secondary text: `#B8B8B8` or brighter; keep essential labels legible. Pure-white text may be used throughout for extra contrast.
- Futura is required throughout: headings, body text, values, chart labels, and footnotes. Use genuine supplied weights; do not synthesize bold or silently substitute another typeface. Use the seven bundled faces in `assets/fonts/` and the metadata-derived weight mappings in `assets/fonts/fonts.css`; see [font setup](../assets/fonts/README.md). Copy assets beside the output or embed their data for standalone HTML. Set `font-synthesis: none` and use only the supplied upright styles. Before PNG export, await `document.fonts.ready` and verify that the Futura font faces loaded successfully.
- Flush-left hierarchy. Big headline, compact takeaway, dominant chart or aligned rows, short footnotes.
- Use whitespace and thin separators instead of nested cards. No gradients, glass effects, decorative glows, ornamental icons, or unnecessary frames.

## Accent colors

More than cyan is allowed. Pick colors for meaning and use them consistently:

| Role | Example color |
| --- | --- |
| General highlight | Cyan `#55E6F2` |
| Primary data series | Blue `#58A6FF` |
| Alternate series / emphasis | Orange `#FF995C` |
| Positive status / third series | Green `#45D6A4` |
| Caution / fourth series | Gold `#F5C451` |
| Negative status | Red `#FF7272` |

Use one accent for simple cards; two to four for real categories or series. Neutrals still carry most text. Do not recolor every sentence. Colored text must remain readable against black. Pair color with labels, order, patterns, or shapes; never make color the only way to tell categories apart. Brand colors are optional only when they are relevant and identifiable.

## Density and sizing

Treat the supplied images as references, not a fixed template. A landscape card around 1200–1600 CSS pixels wide is a useful starting point for charts; short guides may be smaller or square. Prefer a compact landscape composition when the content fits. Do not force tall dense reports into a tiny social preview.

At roughly 1400px wide, try a 44–56px title, 22–28px primary labels, and 18–22px secondary labels. These are starting sizes, not a reason to cram content. Keep captions and caveats readable. Use consistent spacing, roughly 24–48px outer padding and 16–32px between related sections. Export at 2× resolution without confusing export pixels with readable CSS size.

## Chart and table details

- Label values directly. Keep number columns aligned; use tabular numerals.
- Put legends near the chart title when categories need them.
- Show a range with solid lower estimate plus hatching to the upper estimate. Label both endpoints and the denominator.
- Label thresholds, such as 100%, without running their lines through text. Use a black text backing or reposition annotations.
- Stacked bars must reconcile with totals; rounded values may need a concise note.
- Avoid invented precision, unverified savings, or performance claims. A workload ratio is not a price quote; an estimated duration is not a benchmark.
- Thin gray separators can structure rows; chart marks and meaningful boundaries need enough contrast.

## Example selection

Open only the example most relevant to the task initially. Open another if it clarifies a second major visual form. The examples demonstrate design, not required content:

- `examples/quota-and-usage.png`: uncertainty, supporting counts, and cost interpretation.
- `examples/shipping-summary.png`: headline metrics plus chart/table pairing.
- `examples/model-comparison.png`: ranking rows, category accents, score bars, and caveats.

