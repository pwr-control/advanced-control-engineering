# advanced-control-engineering

LaTeX sources of two sets of lecture notes by Davide Bagnara, both compiled as `book`
documents with the shared settings in `AAA_template_latex_settings/`:

- **Advanced Control Engineering: from state-space to nonlinear and optimal methods** —
  the theory and the worked case studies behind the MATLAB/Simulink projects of the
  companion repository
  [lectures-on-advanced-control-engineering](https://github.com/pwr-control/lectures-on-advanced-control-engineering)
  (the same project names are used for the figure folders here);
- **Theory of Electromechanical Devices: collection of main results** — a compact review of
  Maxwell's equations, field analysis and the energy method for electromechanical devices.

Compiled PDFs are tracked next to the sources.

## Repository layout

| Folder | Content |
|---|---|
| [`advanced_control_engineering`](advanced_control_engineering) | `advanced_control_engineering.tex` + PDF: linear system theory, Lyapunov, optimal control, least squares, Kalman, MPC, adaptive control, model derivations and eleven control case studies; `figures/` by topic |
| [`electromechanical_devices`](electromechanical_devices) | `electromechanical_devices.tex` + PDF: Maxwell's equations, magnetostatic field analysis, magnetic circuits, electromechanical energy conversion |
| `AAA_template_latex_settings` | `settings.tex`: packages, page geometry, title-page macros (`\DocTitle`, `\DocAuthor`, `\MetaLabel*`), theorem environments (`defn`, `thm`, `lemma`, `example`, ...) shared by both documents |

Each document folder has its own README with the table of contents.

## Building

From the document folder, e.g. `advanced_control_engineering/`:

```
pdflatex advanced_control_engineering.tex
pdflatex advanced_control_engineering.tex
```

`settings.tex` is included with a relative path (`\input{../AAA_template_latex_settings/settings}`),
so keep the folder structure. Figures are EPS (converted by `epstopdf` at build time) and
PDF; auxiliary files are ignored by git.
