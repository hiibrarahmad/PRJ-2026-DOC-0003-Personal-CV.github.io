<div align="center">

<!-- HEADER BANNER -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1a1a2e,50:16213e,100:0f3460&height=200&section=header&text=Ibrar%20Ahmad%20—%20CV&fontSize=48&fontColor=e94560&fontAlignY=38&desc=Professional%20Curriculum%20Vitae%20·%20LaTeX%20Powered&descSize=18&descAlignY=60&descColor=a8b2d8" width="100%"/>

<!-- BADGES -->
![CV Version](https://img.shields.io/badge/CV%20Version-2026-e94560?style=for-the-badge&logo=latex&logoColor=white)
![Languages](https://img.shields.io/badge/Languages-English%20%7C%20Indonesian-0f3460?style=for-the-badge&logo=googletranslate&logoColor=white)
![Built With](https://img.shields.io/badge/Built%20With-XeLaTeX-16213e?style=for-the-badge&logo=latex&logoColor=white)
![Style](https://img.shields.io/badge/Style-Awesome--CV-e94560?style=for-the-badge&logo=readthedocs&logoColor=white)
![License](https://img.shields.io/badge/License-Personal%20Use%20Only-0f3460?style=for-the-badge&logo=shield&logoColor=white)
![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live-16213e?style=for-the-badge&logo=github&logoColor=white)

<br/>

**[📄 English CV](#-download--view)** · **[🌐 Indonesian CV](#-download--view)** · **[🛠️ Build Guide](#%EF%B8%8F-local-build-guide)** · **[📁 Structure](#-repository-structure)**

</div>

---

## 📖 About This Repository

**Ibrar Ahmad CV** is a professionally maintained, dual-language curriculum vitae repository built with the industry-standard **Awesome-CV** LaTeX template. This repository serves as a single source of truth for both English and Indonesian versions of the CV — version-controlled, reproducible, and ready for deployment via GitHub Pages.

> 💡 Both versions are compiled with **XeLaTeX** for full Unicode and font support, ensuring a polished, professional output every time.

---

## 📄 Download & View

<div align="center">

| Language | Preview | Download |
|:--------:|:-------:|:--------:|
| 🇬🇧 **English** | ![English CV Preview](https://github.com/hiibrarahmad/PRJ-2026-DOC-0003-Personal-CV.github.io/blob/main/cv_english/assets/image.png) | [📥 Download PDF](cv_english/Ibrar_Ahmad_CV_fixed%20(1).pdf) |
| 🇮🇩 **Indonesian** | ![Indonesian CV Preview](https://github.com/hiibrarahmad/PRJ-2026-DOC-0003-Personal-CV.github.io/blob/main/cv_indonesian/assets/image.png) | [📥 Download PDF](cv_indonesian/Ibrar_Ahmad_CV_id.pdf) |

</div>

---

## ✨ What This CV Includes

<div align="center">

| Section | Description |
|:--------|:------------|
| 👤 **Professional Summary** | Concise personal branding statement |
| 💼 **Work Experience** | Roles, responsibilities, and achievements |
| 🎓 **Education** | Academic background and qualifications |
| 🛠️ **Technical Skills** | Languages, tools, frameworks, and platforms |
| 🚀 **Key Projects** | Highlighted personal and professional projects |
| 🏆 **Final Year Project** | Capstone research and engineering work |
| 🌍 **Open-Source Contributions** | Community and GitHub contributions |
| 📜 **Certifications** | Professional and technical credentials |
| 🥇 **Achievements & Recognition** | Awards, honors, and milestones |

</div>

---

## 📁 Repository Structure

```
PRJ-2026-DOC-0003-Personal-CV.github.io/
│
├── cv_english/
│   ├── Ibrar_Ahmad_CV_fixed (1).tex     ← English LaTeX source
│   ├── Ibrar_Ahmad_CV_fixed (1).pdf     ← Compiled English PDF
│   └── awesome-cv.cls                   ← Awesome-CV style class
│
├── cv_indonesian/
│   ├── Ibrar_Ahmad_CV_id.tex            ← Indonesian LaTeX source
│   ├── Ibrar_Ahmad_CV_id.pdf            ← Compiled Indonesian PDF
│   └── awesome-cv.cls                   ← Awesome-CV style class
│
├── .github/
│   └── ISSUE_TEMPLATE/
│       ├── bug_report.md
│       ├── feature_request.md
│       ├── question.md
│       └── config.yml
│
├── index.html                           ← GitHub Pages landing page
└── README.md                            ← This file
```

---

## 🛠️ Local Build Guide

### Prerequisites

| Tool | Purpose | Install |
|:-----|:--------|:--------|
| MiKTeX / TeX Live | LaTeX compiler | [miktex.org](https://miktex.org) |
| XeLaTeX | Unicode-aware compiler | Included with MiKTeX |
| VS Code | Editor | [code.visualstudio.com](https://code.visualstudio.com) |
| LaTeX Workshop | VS Code extension | [Marketplace](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop) |

---

### ⚡ VS Code Setup (Recommended)

**Step 1 — Verify XeLaTeX installation:**
```bash
xelatex --version
```

**Step 2 — Install the VS Code extension:**
> `LaTeX Workshop` by **James Yu**

**Step 3 — Open the `.tex` file for your target language:**
```
cv_english/Ibrar_Ahmad_CV_fixed (1).tex
cv_indonesian/Ibrar_Ahmad_CV_id.tex
```

**Step 4 — Build the PDF:**
```
Ctrl + Alt + B   →  LaTeX Workshop: Build
```

**Step 5 — View the output:**
```
Command Palette → LaTeX Workshop: View LaTeX PDF
```

---

### 🖥️ Manual Build Commands

**English CV:**
```bash
cd cv_english
xelatex -interaction=nonstopmode "Ibrar_Ahmad_CV_fixed (1).tex"
```

**Indonesian CV:**
```bash
cd cv_indonesian
xelatex -interaction=nonstopmode Ibrar_Ahmad_CV_id.tex
```

---

## 🌐 GitHub Pages Deployment

This repository includes an `index.html` landing page for GitHub Pages hosting.

**To deploy:**

1. Push this repository to GitHub
2. Navigate to `Settings → Pages`
3. Set source → **Deploy from branch**
4. Select `main` branch → `/ (root)` folder
5. Click **Save** and wait for deployment ✅

---

## 🐛 Troubleshooting

| Issue | Solution |
|:------|:---------|
| Build does not start | Ensure `xelatex` is in your system PATH · Restart VS Code after MiKTeX install |
| PDF not updating | Save the `.tex` file before building · Re-run build from Command Palette |
| Missing packages | Enable **on-the-fly install** in MiKTeX Console · Rebuild after install |
| Page alignment / spacing | Compile each version from its own folder · Do not mix `.cls` files across folders |

---

## 🤝 Contribution Workflow

- Open issues using templates in `.github/ISSUE_TEMPLATE/`
- Keep changes language-scoped:
  - 🇬🇧 English edits → `cv_english/`
  - 🇮🇩 Indonesian edits → `cv_indonesian/`
- **Rebuild the PDF after every content or layout change**

---

## 📜 License

```
This repository contains personal CV content.
Reuse, redistribution, or modification is only permitted
with explicit written consent from the repository owner.

© 2026 Ibrar Ahmad. All Rights Reserved.
```

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1a1a2e,50:16213e,100:0f3460&height=100&section=footer" width="100%"/>

**Crafted with ❤️ using LaTeX · Awesome-CV · GitHub Pages**

[![GitHub](https://img.shields.io/badge/GitHub-hiibrarahmad-e94560?style=flat-square&logo=github)](https://github.com/hiibrarahmad)

</div>
