# Yoojin Lee Personal Academic Website

This repository contains the static GitHub Pages website for Yoojin Lee.

The site is designed as a clean, minimal academic profile for a bioengineering researcher working in immunoengineering, biomaterials, macrophage biology, and microphysiological systems.

## Local Preview

From the website folder:

```bash
cd ~/Desktop/yoojin
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Deployment to GitHub Pages

1. Create a GitHub repository named `yjinbio.github.io` under the `yjinbio` account.
2. Copy or commit these website files into the repository.
3. Commit and push to GitHub.
4. Enable GitHub Pages if needed. For a user site named `yjinbio.github.io`, GitHub Pages usually serves from the `main` branch automatically.
5. Visit `https://yjinbio.github.io/`.

## First-Time GitHub Deployment Commands

Assuming the repository `yjinbio.github.io` has already been created on GitHub:

```bash
git init
git branch -M main
git add .
git commit -m "Create personal academic website"
git remote add origin https://github.com/yjinbio/yjinbio.github.io.git
git push -u origin main
```

## Files

- `index.html`: Main website content and structure.
- `assets/css/style.css`: Site styling and responsive layout.
- `assets/files/Yoojin_Lee_CV.pdf`: Public CV link used by the website.
- `assets/images/profile/yoojin-lee.jpg`: Profile photo used in the landing section.
- `assets/images/research/`: Placeholder folder for future research figures.

## Manual Updates Still Needed

- Replace the research placeholder images:
  - `assets/images/research/phagocytosis.jpg`
  - `assets/images/research/trogocytosis.jpg`
  - `assets/images/research/mps.jpg`
- Add Google Scholar and ORCID links when available.
- Update `assets/files/Yoojin_Lee_CV.pdf` when the CV changes.
- Add publication links only after publications or preprints are available.
