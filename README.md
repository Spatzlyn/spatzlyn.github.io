# spatzlyn.github.io

Personal site of **Yookyung(Clair) Youn** — undergraduate researcher at Korea University working on robot safety under partial observability.

A single self-contained static page (plain HTML + CSS + vanilla JS, no framework, no build step) with a night-sky theme: canvas starfield, occasional shooting stars, and a cursor-following bird companion.

## Structure

```
index.html            ← the whole site (markup + styles + scripts)
assets/
  fonts/              ← Geist Pixel (Vercel, OFL) — used for the hero name
  img/bird.png        ← cursor-follower character
images/               ← profile photo + favicons
.nojekyll             ← tells GitHub Pages to serve files as-is (no Jekyll build)
```

## Editing

Everything lives in `index.html`:

- **Colors / fonts** — CSS variables in `:root` at the top of the `<style>` block. The hero name font can be switched between the five bundled Geist Pixel variants via `--name-font`.
- **Content** — the About text, Education, Awards, Projects, and Contact sections are plain markup in `<body>`.
- **CV** — to add a Download CV button, place the PDF in the repo (e.g. `files/cv.pdf`) and add an `<a class="cta" href="files/cv.pdf">Download CV →</a>` above `.foot-meta` in the footer.

## Local preview

Open `index.html` directly in a browser, or serve the folder:

```bash
python -m http.server
```
