# PKU Tech Report LaTeX Template

An unofficial LaTeX template for technical reports, preprints, and project reports, featuring the Peking University logo and a red color scheme. This template is adapted from the [Microsoft Tech Report LaTeX Template](https://github.com/lhmd/microsoft-tech-report). It is not an official Peking University template and is not endorsed by the university.

## Quick Start

Upload the project to Overleaf and set `main.tex` as the main document. Alternatively, compile it locally using TeX Live or MacTeX:

```sh
latexmk -pdf -jobname=pku-tech-report main.tex
```

The command generates the sample report as `pku-tech-report.pdf`. The required LaTeX packages are provided by your TeX distribution.

## Customization

- Edit the report title, authors, affiliations, correspondence email addresses, and keywords in `main.tex`. Replace all example names and addresses with your own.
- The title page uses `figures/pku.png` by default. Adjust its size with `\techreportlogoheight{...}`. Follow the university's applicable rules when using its logo.
- Add URLs to `\techreportmeta{Project Page}{...}` and `\techreportmeta{Code}{...}`. Fields with empty values are hidden.
- Replace `\techreportplaceholder{...}` on the first page with `\includegraphics[width=\linewidth]{...}` to add a teaser figure, or remove the entire figure block if it is not needed.
- Edit the abstract and report sections in `sections/`, and manage references in `reference.bib`.
- Adjust the title, links, metadata, abstract box, and other styling in `pku-tech-report.sty`.

## Files

- `main.tex`: Main document and example title page.
- `pku-tech-report.sty`: PKU-themed LaTeX style.
- `figures/pku.png`: Peking University logo supplied with the project.
- `sections/` and `reference.bib`: Example report sections and bibliography.
- `pku-tech-report.pdf`: Compiled example report.
- `NOTICE` and `LICENSE`: Attribution and license information.

## Attribution and License

This template is adapted from the Microsoft Tech Report LaTeX Template by Weijie Wang. The source is distributed under the LaTeX Project Public License, version 1.3c or later. See `NOTICE` and `LICENSE` for attribution and license details. Rights and usage rules for the Peking University logo are separate from the source code license.
