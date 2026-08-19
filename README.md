# Zhining Sun — Academic Website

Static academic website for GitHub Pages.

## Live-site repository

This project is set up for the GitHub account:

`agecon-zhiningsun`

This package is configured for your existing repository:

`zs.github.io`

Because the repository name is different from your GitHub username, GitHub Pages will publish it as a project site at:

`https://agecon-zhiningsun.github.io/zs.github.io/`

## What is included

- About/home page
- Research page
- Publications and working papers
- Teaching
- Extension/outreach
- Data & Code
- Current CV at `assets/Zhining_Sun_CV.pdf`
- Responsive navigation
- An RStudio project file for convenient editing
- No build step and no R packages required

## Publish for the first time

1. Keep your existing repository name as `zs.github.io`. No rename is needed.
2. Upload **the contents of this folder** to the repository root. `index.html` must be directly in the repository root.
3. Commit the files to `main`.
4. In GitHub, go to **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Choose branch `main` and folder `/ (root)`, then save.
7. Open `https://agecon-zhiningsun.github.io/zs.github.io/` after deployment finishes.

## Recommended way to update later: RStudio + Git

R is **not** used to build the website. RStudio is simply a convenient editor and Git interface.

### One-time local setup

Clone the repository to your computer:

```bash
git clone https://github.com/agecon-zhiningsun/zs.github.io.git
```

Then open:

`zs.github.io.Rproj`

in RStudio.

### Every time you update the site

1. Open the `.Rproj` file in RStudio.
2. Edit the relevant HTML file.
3. Save.
4. In RStudio's **Git** tab, stage the changed files.
5. Click **Commit** and enter a short message, e.g. `Update publications`.
6. Click **Push**.
7. GitHub Pages will redeploy the site automatically.

### Which file to edit

- `index.html` — bio, title, contact info, What's New
- `research.html` — research fields and working papers
- `publications.html` — publications and working papers
- `teaching.html` — teaching
- `extension.html` — extension/outreach and media
- `data.html` — data and code
- `assets/style.css` — fonts, spacing, layout, visual design
- `assets/headshot.webp` — profile photo
- `assets/Zhining_Sun_CV.pdf` — current CV

## Update the CV later

Export the new CV PDF from Overleaf, rename it exactly:

`Zhining_Sun_CV.pdf`

Then replace:

`assets/Zhining_Sun_CV.pdf`

with the new PDF. Because the filename stays the same, **you do not need to edit any website links**. Commit and push the replacement PDF.

## Add a publication later

Open `publications.html`, copy one existing `<article class="paper"> ... </article>` block, paste it where you want the new paper, and change its title/authors/venue/link. Save, commit, and push.

## Preview locally

The easiest check is simply to open `index.html` in a browser.

If you want a local web server, from the project folder you can run in a terminal:

```bash
python -m http.server 8000
```

and then open `http://localhost:8000`.

## File structure

```text
.
├── index.html
├── research.html
├── publications.html
├── teaching.html
├── extension.html
├── data.html
├── 404.html
├── zs.github.io.Rproj
├── .nojekyll
├── .gitignore
├── README.md
└── assets/
    ├── style.css
    ├── site.js
    ├── headshot.webp
    └── Zhining_Sun_CV.pdf
```
