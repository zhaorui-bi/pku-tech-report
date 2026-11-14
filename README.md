# PKU Tech Report LaTeX Template

An unofficial technical report template featuring the Peking University logo
and a red color scheme. Its research-article organization draws on general
Nature Portfolio guidance, while retaining a technical report title page. It is
not an official university or journal template.

## Getting Started

Upload the project files to Overleaf and select `main.tex` as the main file.
To build locally with a TeX distribution and `latexmk`, run:

```sh
latexmk -pdf -jobname=pku-tech-report main.tex
```

## Customize the Report

- Edit the title, authors, affiliations, contact, and keywords in `main.tex`.
- Change the logo height in `\ReportHeader{figures/pku.png}{0.9cm}`.
- Replace `\ReportTeaserPlaceholder{...}` with `\includegraphics[width=\textwidth]{...}` to add a graphical abstract.
- Edit the abstract and the Introduction, Results, Discussion, Conclusion, and Methods files in `sections/`. Write Results subsection titles as findings supported by the study's evidence.
- Replace the placeholders in `sections/06_availability.tex` and `sections/07_declarations.tex` with accurate statements, or adjust them to the target journal's requirements.
- Add main-text references to `reference.bib` and cite them with `\cite{...}`. References use numbered superscript citations in order of appearance.
- Customize `sections/08_supporting_information.tex`. Change each section title in its `\SITitle...` command; add or remove both the table-of-contents entry and matching section together. Section numbers and page numbers update on recompilation. Supplementary figures and tables use S-prefixed numbering. Supplementary references are a manually maintained list, separate from the main bibliography.
- For review line numbers, add `\usepackage{lineno}` in the preamble and `\linenumbers` after the title page. Adjust line spacing, graphical abstract, section order, and separate supplementary files as required by your chosen journal.
- Adjust colors and typography in `pku-tech-report.sty`.

## Submission Guidance

Requirements vary by journal and article type. Before submission, check the
journal's current instructions for abstract length, manuscript order, figures,
references, declarations, reporting summaries, and supplementary information.
This report template does not guarantee compliance with a particular journal.
Useful starting points are [Nature Portfolio's writing guidance](https://www.nature.com/nature-portfolio/for-authors/write)
and [reporting and availability policies](https://www.nature.com/nature-portfolio/editorial-policies/reporting-standards).

## License

The template code and documentation are available under the MIT License. The
university name and logo are excluded and may have separate usage restrictions;
see `NOTICE`.
