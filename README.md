# Ibrar Ahmad CV (LaTeX)

Professional CV repository with two maintained versions:
- `cv_english/` for English CV
- `cv_indonesian/` for Indonesian CV

Both versions use the Awesome-CV style and are structured for local editing, VS Code workflow, and GitHub hosting.

## Repository Structure

```text
.
├── cv_english/
│   ├── Ibrar_Ahmad_CV_fixed (1).tex
│   ├── Ibrar_Ahmad_CV_fixed (1).pdf
│   └── awesome-cv.cls
├── cv_indonesian/
│   ├── Ibrar_Ahmad_CV_id.tex
│   ├── Ibrar_Ahmad_CV_id.pdf
│   └── awesome-cv.cls
├── .github/
│   └── ISSUE_TEMPLATE/
│       ├── bug_report.md
│       ├── feature_request.md
│       ├── question.md
│       └── config.yml
├── index.html
└── README.md
```

## What This CV Includes

- Professional summary
- Experience
- Education
- Technical skills
- Key projects
- Final year project
- Open-source contributions
- Certifications
- Achievements and recognition

## Why This Repo Is Useful

- Single source of truth for both language versions
- Easy to maintain with LaTeX versioned files
- Reproducible PDF builds using XeLaTeX
- Ready for GitHub Pages documentation and issue tracking

## Prerequisites

- MiKTeX or TeX Live with `xelatex`
- Visual Studio Code
- VS Code extension: `LaTeX Workshop`

## VS Code Setup (Recommended)

1. Install MiKTeX (or TeX Live) and verify:
   - `xelatex --version`
2. Install VS Code extension:
   - `LaTeX Workshop` by James Yu
3. Open this repository in VS Code.
4. Open a `.tex` file from either folder:
   - `cv_english/Ibrar_Ahmad_CV_fixed (1).tex`
   - `cv_indonesian/Ibrar_Ahmad_CV_id.tex`
5. Build:
   - `Ctrl+Alt+B` (LaTeX Workshop build)
   - or Command Palette: `LaTeX Workshop: Build LaTeX project`
6. View PDF:
   - Command Palette: `LaTeX Workshop: View LaTeX PDF`
   - enable auto-refresh for live preview behavior

## Manual Build Commands

English:
```powershell
cd cv_english
xelatex -interaction=nonstopmode "Ibrar_Ahmad_CV_fixed (1).tex"
```

Indonesian:
```powershell
cd cv_indonesian
xelatex -interaction=nonstopmode Ibrar_Ahmad_CV_id.tex
```

## Troubleshooting

- Build does not start:
  - Ensure `xelatex` is in PATH
  - Restart VS Code after MiKTeX install
- PDF not updating:
  - Save the `.tex` file before build
  - Re-run build manually from Command Palette
- Missing packages:
  - In MiKTeX Console, enable on-the-fly install
  - install missing package and rebuild
- Page alignment / spacing:
  - Keep each language version compiled from its own folder
  - avoid mixing `.cls` across folders

## GitHub Pages Docs

- `index.html` is provided as a documentation landing page.
- For GitHub Pages:
  1. Push this repo to GitHub
  2. Open `Settings > Pages`
  3. Set source to `Deploy from branch`
  4. Select `main` and `/ (root)`
  5. Save and wait for deployment

## Contribution Workflow

- Open issues using templates in `.github/ISSUE_TEMPLATE/`
- Keep changes language-scoped:
  - English edits in `cv_english/`
  - Indonesian edits in `cv_indonesian/`
- Rebuild PDF after every content or layout edit

## License

This repository contains personal CV content. Reuse only with permission from the owner.
