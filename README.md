# PKU Tech Report LaTeX Template

An unofficial technical report template featuring the Peking University logo
and a red color scheme. It is suitable for reports, preprints, and research
notes. This project is not endorsed by Peking University.

## Getting Started

Upload the project files to Overleaf and select `main.tex` as the main file.
To build locally with a TeX distribution and `latexmk`, run:

```sh
latexmk -pdf -jobname=pku-tech-report main.tex
```

## Customize the Report

- Edit the title, author names, affiliations, contact, and keywords in `main.tex`.
- Change the logo height in `\ReportHeader{figures/pku.png}{0.9cm}`.
- Replace `\ReportTeaserPlaceholder{...}` with `\includegraphics[width=\textwidth]{...}` to display a figure.
- Edit the abstract and other sections in `sections/`.
- Add references to `reference.bib` and cite them with `\cite{...}`.
- Adjust colors and typography in `pku-tech-report.sty`.

## License

The template code and documentation are available under the MIT License. The
university name and logo are excluded and may have separate usage restrictions;
see `NOTICE`.
