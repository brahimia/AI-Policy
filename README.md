# Personal website — Babak Rahimi Ardabili

A static site (plain HTML/CSS/JS, no build step) ready for GitHub Pages.

## Deploying on GitHub Pages

1. Create a new GitHub repository. If you want it at `https://<username>.github.io`, name the repo exactly `<username>.github.io`. Otherwise any repo name works and your site will be at `https://<username>.github.io/<repo-name>`.
2. Upload these files to the repo root: `index.html`, `styles.css`, `script.js`, and the `assets/` folder (keep the CV PDF inside `assets/`).
3. In the repo, go to **Settings → Pages**.
4. Under **Build and deployment → Source**, choose **Deploy from a branch**.
5. Under **Branch**, choose `main` (or `master`) and folder `/ (root)`, then **Save**.
6. Wait a minute or two — GitHub will give you the live URL at the top of that same Pages settings screen.

## Before you publish — things to update

- **LinkedIn and Google Scholar links** in `index.html`: search for `linkedin.com` and `scholar.google.com` and replace the placeholder URLs with your real profile links (search for `href="https://linkedin.com"` and `href="https://scholar.google.com"`).
- **Contact email**: currently `brahimia@charlotte.edu` — update if this changes after graduation.
- Swap `assets/Babak_Rahimi_Ardabili_CV.pdf` for a fresh export whenever your CV updates — the filename can stay the same so no links break.

## Editing content later

Everything is in `index.html`, organized by section with HTML comments (`<!-- RESEARCH -->` etc). No templating system — just find the section and edit the text directly. Colors, fonts, and spacing all live in `styles.css` under the `:root` block at the top if you want to adjust the palette.

## Local preview

Just double-click `index.html` to open it in a browser, or from this folder run:

```
python3 -m http.server 8000
```

and visit `http://localhost:8000`.
