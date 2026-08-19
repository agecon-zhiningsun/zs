# Quick Website Update Guide

## Normal update workflow in RStudio

1. Double-click `zs.github.io.Rproj`.
2. Edit the page you want.
3. Save it.
4. Open the **Git** tab.
5. Check the box beside each changed file.
6. Click **Commit**.
7. Write a message such as `Update CV` or `Add new publication`.
8. Click **Commit** in the commit window.
9. Click **Push**.
10. Wait for GitHub Pages to redeploy, then refresh the live website.

## Replace the CV

1. Download/export your newest PDF from Overleaf.
2. Rename it `Zhining_Sun_CV.pdf`.
3. Replace `assets/Zhining_Sun_CV.pdf`.
4. Commit and push.

No HTML edit is needed when the filename stays the same.

## Add a paper

Edit `publications.html` and duplicate an existing paper block:

```html
<article class="paper">
  <p class="paper-title"><a href="YOUR-LINK" target="_blank" rel="noopener">Paper Title</a></p>
  <p class="paper-authors"><strong>Zhining Sun</strong>, Coauthor</p>
  <p class="paper-venue"><em>Journal Name</em>, year.</p>
  <p class="paper-links"><a href="YOUR-LINK" target="_blank" rel="noopener">DOI</a></p>
</article>
```

## Change the homepage news

Edit the `What's New` section in `index.html`. Copy an existing `news-item` block and change the date/text.

## Change the photo

Replace `assets/headshot.webp` with another image using the same filename. If you use a different filename or extension, also change the image path in `index.html`.


## Repository and live URL

- GitHub repository: `https://github.com/agecon-zhiningsun/zs.github.io`
- Live website: `https://agecon-zhiningsun.github.io/zs.github.io/`

Keep the repository name `zs.github.io`; you do not need to rename it.
