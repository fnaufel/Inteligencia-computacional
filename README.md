# Understanding Deep Learning presentations

This is a Quarto project for Reveal.js presentations based on *Understanding Deep Learning* by Simon Prince. Each chapter has its own directory under `chapters/`. Shared presentation settings live in `_quarto.yml`, shared styling lives in `shared/theme/`, and the Quarto extensions used by the slides live in `_extensions/`.

## Render

From the project root, run `quarto render` to build every chapter or `quarto render chapters/04-deep-networks/slides.qmd` to build chapter 4 alone. Open `_output/chapters/04-deep-networks/slides.html` after rendering. The default is `embed-resources: false`, so distribute the HTML together with its generated `slides_files/`, `assets/`, and shared style files from `_output/`.

The `_output/` directory contains generated files and is ignored by Git. Source files, licensed artwork, and the original PowerPoint for chapter 4 are described in [the chapter README](chapters/04-deep-networks/README.md).

## Add a chapter

Create `chapters/NN-topic/slides.qmd` and place chapter-specific artwork beside it in `assets/`. The project render list picks up files named `slides.qmd` in chapter directories. Put a file in `shared/` only when multiple presentations use it, and keep the applicable license with any third-party artwork.
