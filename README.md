# PRB Manuscript Folder

This folder is a self-contained `RevTeX 4.2` / `PRB` manuscript project for the interacting Lieb-Kitaev chain.

Project structure:

- `main.tex`: manuscript entry point
- `refs.bib`: bibliography
- `figures/selected/`: figures actually referenced by the paper
- `data/selected_curves/`: copied raw text curves matching the selected figures
- `FIGURE_SOURCES.md`: provenance map from the manuscript figures back to the original analysis directory

Recommended compile sequence on `latex.sjtu.edu.cn`:

```text
pdflatex main
bibtex main
pdflatex main
pdflatex main
```

Notes:

- The current draft follows strict `PRB` sectioning and RevTeX syntax.
- The results section is built around the copied `1-18-analysis` figures, especially the bulk-averaged orbital occupation versus `U`.
- Local compilation was not performed here because `pdflatex` and `bibtex` are not installed in the current environment.
