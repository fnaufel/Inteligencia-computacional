# Chapter 4: Deep Neural Networks

`slides.qmd` is the active Reveal.js presentation. Render it from the project root with `quarto render chapters/04-deep-networks/slides.qmd`. Shared Reveal.js settings, including `embed-resources: false`, are in the root `_quarto.yml`.

## Files

- `assets/book-svg-originals/` contains the nine original Chapter 4 SVGs and their `LICENSE.txt`. Slides use these files directly where applicable.
- `assets/figures/` contains derived artwork and raster images used by the slides.
- `assets/sequences/` contains the frames used by the graphical build-up animation.
- `source/04_Deep.pptx` is the original PowerPoint used for this conversion.
- `source/figure_manifest_v4.csv` records the author SVG to PowerPoint mapping from the earlier conversion; its “V4 use” column is historical and does not describe every image in the current slides.

The deck uses editable LaTeX expressions and selected vector artwork in place of many PowerPoint image exports. It is a content conversion rather than a pixel-exact copy of the PowerPoint. The original book artwork remains subject to the license in `assets/book-svg-originals/LICENSE.txt`.

The composition sequence is a reconstructed vector animation based on the original Chapter 4 SVGs. The linear-region plots use the analytical formula, while one slide retains the PowerPoint caption of 161,501 regions for the five-layer, ten-unit example; the formula gives 161,051. The complete `DeepTwoLayer.svg` replaces a truncated PowerPoint diagram.

The earlier raster-based Quarto conversion and unused fallback exports were removed from the working tree after validating this deck. They remain available in Git history.
