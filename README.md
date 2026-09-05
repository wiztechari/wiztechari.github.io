# Hari Krishnan — Portfolio

A single-page, terminal/IDE-themed developer portfolio. Static HTML/CSS/JS — no build step, no dependencies to install.

## Files

- `index.html` — the entire site (structure, styles, and script in one file)
- `resume.pdf` — downloadable resume, linked from the hero and contact sections

## Deploy to GitHub Pages

1. Create a new repository (or use an existing one), e.g. `wiztechari/wiztechari.github.io` for a user site, or any repo name for a project site.
2. Push these two files to the repo root:
   ```bash
   git init
   git add index.html resume.pdf
   git commit -m "Add portfolio site"
   git branch -M main
   git remote add origin https://github.com/wiztechari/YOUR-REPO-NAME.git
   git push -u origin main
   ```
3. In the repo on GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, then pick branch `main` and folder `/ (root)`. Save.
4. Your site will be live at:
   - `https://wiztechari.github.io/YOUR-REPO-NAME/` (project site), or
   - `https://wiztechari.github.io/` (if the repo is named `wiztechari.github.io`)

## Customizing

- **Update content**: edit the text directly inside `index.html` — the `about`, `skills`, `projects`, and `contact` sections are clearly marked with HTML comments-equivalent `<section id="...">` blocks.
- **Swap the resume**: replace `resume.pdf` with your own file, keeping the same filename (or update the `href="resume.pdf"` links in `index.html` if you rename it).
- **Colors**: all colors are CSS variables at the top of the `<style>` block (`:root { --bg: ...; --accent: ...; }`) — change them once and the whole site updates.
- **Add a project**: copy one `<article class="project">...</article>` block in the `#projects` section and edit its filename, description, and stack line.
