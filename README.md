# James Diamantis — Engineering Portfolio

A static, no-build website (plain HTML/CSS) covering two Northeastern Cornerstone of
Engineering projects: the **OceanGate disaster investigation** (GE1501) and the
**EasyDose automated pill dispenser** (GE1502).

## Files

- `index.html` — the whole site (single page, anchor-linked sections)
- `style.css` — all styling
- `assets/` — images, all real photos/renders from the project reports:
  - `oceangate-hero.jpg` — the Stage 1 Pico breadboard prototype (LEDs + buzzer)
  - `oceangate-cad.jpg` — your AutoCAD laser-cutting pattern for the Stage 2 enclosure
  - `easydose-hero.jpg` — the finished EasyDose enclosure (front view)
  - `easydose-internals.jpg` — CAD render of the tube-and-cup dispensing mechanism
  - `easydose-iteration.jpg` — the original funnel-and-ramp concept render (v1)
  - To swap any image later, just replace the file — same filename, page updates automatically.
- `.nojekyll` — tells GitHub Pages to serve the files as-is (no Jekyll processing needed)

## Deploying to GitHub Pages (free, ~5 minutes)

1. Go to [github.com/new](https://github.com/new) and create a new repository.
   - If you want it at `https://<your-username>.github.io`, name the repo exactly
     `<your-username>.github.io`. Otherwise any name works and it'll deploy to
     `https://<your-username>.github.io/<repo-name>`.
   - Keep it **Public**.
2. Upload these files into the repo:
   - Easiest way: on the repo's GitHub page, click **Add file → Upload files**, then
     drag in `index.html`, `style.css`, `.nojekyll`, and the whole `assets/` folder.
   - Or, if you use git locally:
     ```
     git init
     git add .
     git commit -m "Initial portfolio"
     git branch -M main
     git remote add origin https://github.com/<your-username>/<repo-name>.git
     git push -u origin main
     ```
3. In the repo, go to **Settings → Pages**.
4. Under "Build and deployment", set **Source** to `Deploy from a branch`, branch
   `main`, folder `/ (root)`. Save.
5. GitHub will give you a live URL (usually live within a minute or two) — that's your
   portfolio link, shareable with anyone.

## Editing later

Everything is plain HTML/CSS — no build tools, no npm install. Open `index.html` in
any text editor (or right in GitHub's web editor) to change text; swap files in
`assets/` to change images. Push your changes and the live site updates automatically.
