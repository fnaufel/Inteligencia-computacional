# CM20315 — Deep Neural Networks: Quarto Reveal.js conversion (revision 2)

Original source: `CM20315_04_Deep.pptx` — **66 PowerPoint slides**, Prof. Simon Prince.

## Contents

- `CM20315_04_Deep.qmd` — **39 Reveal.js slides**, written in Markdown and LaTeX.
- `figures/` — **43 individual non-equation PNG figures** from the original PowerPoint. This includes diagrams, plots, the Bath logo and feedback QR code; some diagrams contain mathematical labels.
- `math_fallback/` — **65 original PNG equation images**, retained for reference only. **None are embedded in the QMD.**
- `slide_assets/` — **25 full-canvas PNG frames** for the two original graphical build-up sequences.
- `figure_manifest.csv` — maps the 108 original images to their source PowerPoint slides, shape metadata and current filename.
- `slide_map.csv` — maps merged PowerPoint slide ranges to their Reveal.js slide positions.

## Rendering

With Quarto installed, run in this directory:

```sh
quarto render CM20315_04_Deep.qmd --to revealjs
```

Open the resulting `CM20315_04_Deep.html`. Do not move the image directories before rendering. The QMD uses the built-in Quarto Reveal.js defaults, **no custom CSS**, **no raw HTML**, and only standard Quarto/Pandoc fenced-div syntax for r-stack fragments.

## Original PowerPoint animations

- Original **6–26**: 21 graphic frames become one `r-stack` Reveal.js slide, each image a fragment.
- Original **38–41**: 4 graphic frames become one `r-stack` Reveal.js slide, each image a fragment.
- Original **45–48**: equation-image build-up becomes one 4-fragment **LaTeX** `r-stack` slide. The original equation pictures remain in `math_fallback/`, and are not shown.
- Original **50–51**: the explanatory math labels become one 2-fragment **LaTeX** `r-stack` slide, again without equation images.

Advance through a stack with the next-fragment control (typically Space or Right Arrow).

## Fidelity and limits

- Mathematical expressions have been **manually transcribed** to LaTeX as closely as possible from the original imagery, sometimes using vector/sum notation to avoid unreadably long formulas. The fallback files allow visual comparison with the original formulas.
- Text and diagrams were restructured for default Reveal.js layout; precise PowerPoint positions and decorative styling were not reproduced.
- The diagram/plot animation frames intentionally keep the original plot axes and labels intact, and are not equation-only screenshots.
- The presentation was validated with Pandoc's Reveal.js writer (39 sections, 4 `r-stack` blocks), and all file references were checked. Quarto was not installed in the conversion environment, so a full `quarto render` could not be performed.
