# CM20315 — Deep Neural Networks (Quarto Reveal.js, v4)

## Usage

Unzip the archive, then run:

```bash
quarto render CM20315_04_Deep.qmd
```

The Quarto file uses **Reveal.js default styling** and **Markdown** throughout, with Quarto/Pandoc fenced divs for `r-stack` and the animations. No `.css` file or raw HTML layout is required.

## What changed in v4

The original **nine Chapter 4 author SVGs** from the supplied `Chap04.zip` are in `book_svg_originals/` (with the original license). Author vector artwork replaces several PPT raster diagrams: network composition, folding, 2D composition, two-layer network, K-layer network, and the build-up plots.

- **Animation PPT 6–26:** a 21-step vector animation, based on `DeepConcatQuestion.svg` and `DeepConcat.svg`, with vector cursor positions illustrating progression. These are newly constructed frames, not pixel-exact reproductions of the PowerPoint's moving markers.
- **Animation PPT 38–41:** four progressive SVG crops of the author's `DeepBuildUp.svg`, in one `r-stack` slide.
- **Figures PPT 58–59:** vector reconstructions using the Chapter 4 analytical formula for the number of linear regions; the captions retain the original PPT numbers. The source contains a small numerical discrepancy for the 1D five-layer example: `(10+1)^5 = 161,051`, whereas the PowerPoint prints `161,501`. The plot is computed from the formula.
- **Truncated diagram PPT 37:** replaced with complete author SVG `DeepTwoLayer.svg`.
- The editor-ready **LaTeX expressions** remain in the `.qmd` (see the publisher's source at https://github.com/udlbook/udlbook/blob/main/UDL_Equations.tex).

## Files

- `CM20315_04_Deep.qmd` — presentation source.
- `figures/` — the SVG and PNG images actually used in the deck.
- `slide_assets/author_sequences/` — SVG frames for the two Reveal.js animations.
- `book_svg_originals/` — the nine unmodified author SVGs and their license, for further editing.
- `math_fallback/` — equation graphics from the original PPT, **not displayed** in the deck.
- `raster_fallback/`, `animation_fallback/` — previous figure and frame exports, **not displayed** in the deck.
- `figure_manifest_v4.csv` — author SVG to PPT slide mapping.

## Validation and caveats

The QMD and all image references were checked and the author SVGs rendered into previews. If Quarto is not installed in the execution environment, a full browser-level Reveal.js rendering cannot be guaranteed. The slides are a faithful **content** conversion, not a pixel-exact reproduction of the PowerPoint artwork; while numerous images are now resolution-independent vectors, some non-Chapter-4 raster images remain (e.g., a training chart and feedback QR).

Sources: supplied `CM20315_04_Deep.pptx`, supplied Chapter 4 SVG archive, publisher's Chapter 4 equation source. Figures remain subject to the original book's license (included in the archive).
