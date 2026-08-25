# myResume

LaTeX source for my resume, built on a classic single-column template
(`article` class, custom `\resume*` macros for consistent formatting).

## Build

```bash
pdflatex resume.tex
```

Requires a standard TeX Live distribution (uses `titlesec`, `enumitem`,
`hyperref`, `fancyhdr`, `tabularx`, `marvosym`, `glyphtounicode`).

## Structure

- `resume.tex` — main source file
- `resume.pdf` — compiled output

## License

Personal use only — feel free to reference the formatting macros, but
please don't reuse my content.
