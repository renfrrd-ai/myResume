# myResume

LaTeX source for my resume, built on a classic single-column template
(`article` class, custom `\resume*` macros for consistent formatting).
Visible at https://renfred.dev/resume

## Build

```bash
pdflatex resume.tex
pdflatex resume.tex
```

Run it twice — the first pass writes the `hyperref` link targets, the second
resolves them. Output is `resume.pdf` in the same directory.

### Dependencies

Beyond a base TeX install, the preamble pulls in `fullpage` (from the
`preprint` bundle), `titlesec`, `enumitem` and `marvosym`. On Debian/Ubuntu
these are *not* part of `texlive-latex-base`:

```bash
sudo apt install texlive-latex-extra texlive-fonts-extra
```

The rest (`latexsym`, `color`, `verbatim`, `hyperref`, `fancyhdr`, `babel`,
`tabularx`, `glyphtounicode`) ship with a base install.

If you can't install system-wide, the same four packages work from a user
tree at `~/texmf` using the TDS layout (`~/texmf/tex/latex/<pkg>/`), which
`pdflatex` picks up with no extra configuration.

## Structure

- `resume.tex` — main source file
- `resume.pdf` — compiled output
- `research/` — research-focused version (Research section first, for roles like Google Student Researcher). Build it the same way from inside `research/`.
- `pinterest/` — tailored for the Pinterest Software Engineering Intern role (Toronto, Summer 2027): uofthub first, coursework and AI-assisted development keywords. Build it the same way from inside `pinterest/`.

## License

Personal use only — feel free to reference the formatting macros, but
please don't reuse my content.
