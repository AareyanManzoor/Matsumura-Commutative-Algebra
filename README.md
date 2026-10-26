# Matsumura-Commutative-Algebra
This it the TeX of Matsumura Commutative Algebra, TeX'd by the TeXromancers

The source began as our first Overleaf project. The current revision restores source discrepancies against Matsumura's *Commutative Algebra*, second edition (1980), including the separate Index of Symbols. Corrections of mathematical and reference errors inherited from that edition are explicitly distinguished in editorial notes and the new-typesetting preface. The EGA citations identify the relevant fascicles, and Northcott's *Finite Free Resolutions* has its correct bibliographic record.

Feel free to download and change for example font to better fit your preferences. Your can report errors to my email at amanzoo1 at asu dot edu, or at my discord JohnDS#1149, or as changes to this github with documentation of what was changed.

Link to book: https://aareyanmanzoor.github.io/assets/matsumura-CA.pdf

Link to dyslexic friendly version: https://aareyanmanzoor.github.io/assets/matsumura-CA-dyslexic.pdf

## Building

Use a current TeX Live installation with pdfLaTeX, Biber (compatible with the installed `biblatex`), MakeIndex and `latexmk`. From this directory run:

```sh
latexmk -pdf -interaction=nonstopmode -halt-on-error -outdir=build main.tex
```

Keep the bibliography backend as Biber; `latexmk` runs the bibliography, index and repeated LaTeX passes needed to resolve references. The resulting PDF is `build/main.pdf`. Generated files in `build/` are not source files and should not be committed. The optional dyslexic-font input remains commented out in `main.tex`.
