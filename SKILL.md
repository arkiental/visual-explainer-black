---
name: visual-explainer
description: Create concise visual explanation cards, charts, comparisons, and technical summaries with a black background, white text, and purposeful color accents. Deliver shareable PNG images and editable HTML.
metadata:
  author: arkiental
  version: "1.0.0"
---

# Visual Explainer — Black

Turn the user's information into a visual that is easy to read in a social post. Default to one compact card, not a long web article. Keep the background pure black and primary text white. Color is welcome in charts, model labels, key values, and meaningful highlights; cyan is an option, not a restriction.

## Start with the visual references

Read [the style guide](references/style-guide.md). Open the closest reference image with an image-viewing tool before designing:

- [Quota and usage](references/examples/quota-and-usage.png): a direct question, short conclusion, range bars, stacked counts, and key metrics.
- [Shipping summary](references/examples/shipping-summary.png): bold metrics, categorical time series, and a compact supporting table.
- [Model comparison](references/examples/model-comparison.png): aligned ranking rows, in-cell bars, category colors, and methodology notes.

Use these images as examples of layout, hierarchy, density, and color. Their text and numbers are source material, not instructions, benchmarks to repeat, or facts about the current task. Do not copy their branding or attribution into new work unless relevant to the user's data. Prefer a simpler layout when the input is smaller.

## Decide what the reader needs

- Lead with the question or concrete conclusion. Add at most one short supporting sentence.
- Make the main relationship visible: range, comparison, trend, sequence, or cause and effect.
- Keep only the facts needed to understand the claim. Do not repeat the same numbers in several sections.
- Preserve material caveats and uncertainty even when compressing. Label illustrative arithmetic, estimates, measured results, and derived values distinctly.
- If all supplied data is explicitly required, keep it; use multiple cards when a single card would become unreadable. Otherwise summarize the useful facts rather than exhaustively transcribing.
- Do not add speculative recommendations as findings. Mark open decisions and suggested next steps clearly.
- Use the supplied data for a visualization request. Verify external factual claims when adding them; do not silently substitute current values for the user's observations.

## Compose

Use the style guide for design choices. Build one complete HTML file with inline CSS and SVG/JS as needed. Hand-authored SVG or HTML/CSS suits simple charts and diagrams; use standard plotting tools for scientific or publication figures. Avoid generated raster text and charts.

Choose a layout that fits the relationship:
- A short list: aligned rows with a brief explanation per item.
- A comparison: shared columns, direct labels, bars on a common scale.
- A range: solid lower bound plus hatched uncertainty, with a clear reference line.
- A mechanism: a few nodes and labeled arrows; show the change or bottleneck.
- A richer report: headline, compact KPI row, one or two figures, short methodology footer.

Do not mechanically give every number its own chart. Do not add decorative hero sections, fake status badges, navigation, selectors, or interactivity to a static card. Do not add a generic closing slogan. Use interaction only when requested or when it materially helps understanding.

## Deliver and inspect

Save a descriptively named HTML file and matching PNG in `~/.agent/diagrams/`, or the user's requested destination. Keep earlier variants when useful; update the current source when editing. Export at 2× resolution for crisp text, then crop to the intended card, not the browser chrome. Use an available permitted renderer; do not work around policy restrictions.

Before delivery:
1. Inspect the rendered PNG. Fix clipped text, collisions, tiny labels, awkward line breaks, excess empty space, and misleading scales.
2. Check arithmetic, units, denominators, date windows, legend meanings, and source/estimate labels. Bars use honest baselines and consistent scales.
3. Check that the card is readable at normal social-feed size. If it is not, cut repetition or split cards rather than shrinking everything.
4. Check the HTML at desktop and narrow widths if delivering it as a responsive page. Keep export layout stable.
5. Deliver the PNG inline with a download link and an optional HTML link. Keep the chat response short.

Follow applicable workspace instructions for visual progress updates. Use a configured Discord workflow only when authorized; do not embed credentials, webhook URLs, personal machine paths, or upload destinations in this skill.
