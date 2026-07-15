# David Xchel Morales Hurtado — CV (LaTeX Project)

Self contained LaTeX source code for my CV.

## Build instructions
This project requires **XeLaTeX** (needed for the `fontspec`-loaded font, Carlito).

```bash
xelatex resume.tex
```

Required packages (all in a standard TeX Live install): `fontspec`, `geometry`,
`parskip`, `xcolor`, `titlesec`, `enumitem`, `tabularx`, `array`, `hyperref`.

## Design notes
- Font: **Carlito** (metric-compatible with Calibri) via `fontspec` — clean,
  modern, ATS-safe (no ligatures/icons that confuse parsers).
- Color palette: deep navy (`#0B3D5C`) for headings/name, muted teal (`#2E7D6B`)
  for rules and job titles — professional.
- Single-column layout for maximum ATS (applicant tracking system) compatibility.
  No tables-as-layout, no icons/graphics that conflicts with OCR/parsers
  (`tabularx` blocks used for Skills/Courses are simple two-column text tables,
  which parse fine).
