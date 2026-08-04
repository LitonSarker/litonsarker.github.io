# litonsarker.github.io

Liton Sarker's personal academic portfolio, rebuilt as a Jekyll site using the
[AcademicPages](https://github.com/academicpages/academicpages.github.io) structure
(a fork of [Minimal Mistakes](https://mademistakes.com/work/minimal-mistakes-jekyll-theme/)),
with content migrated from the previous Google Site
(https://sites.google.com/view/litonsarker/).

This build uses Minimal Mistakes as a **remote theme** (`remote_theme: mmistakes/minimal-mistakes`)
rather than vendoring the full theme source, so GitHub Pages can build it directly — no local Ruby
install required to publish, though one is recommended for previewing changes.

## What's inside

- `_config.yml` — site settings, nav, author/social links, collections
- `_pages/` — About (home), CV, Experience, Publications, Talks, Portfolio index pages
- `_publications/` — the two IEEE papers (EF-SwinNet, ADTNet)
- `_talks/` — the ASCE CI Summit 2025 poster presentation
- `_portfolio/` — 7 project write-ups (Revit API Automation, 3D PointNet++, welfare MIS,
  HR-PMS, 4G analytics, Huawei SDM rollout, Robi OSS/NMS deployment)
- `_data/navigation.yml` — top nav menu
- `images/` — empty; add your headshot and project images (see `images/README.md`)

## Publish it on litonsarker.github.io

You said you already created the `litonsarker.github.io` repo on GitHub — to make it live:

1. Download/unzip this folder locally.
2. Copy every file (including hidden ones like `.gitignore`) into your local clone of
   `litonsarker.github.io`, overwriting what's there.
3. From inside that folder:
   ```bash
   git add -A
   git commit -m "Rebuild site with AcademicPages structure"
   git push origin main
   ```
4. In the GitHub repo, go to **Settings → Pages** and confirm the source is set to deploy from
   the `main` branch (root). GitHub Pages will build automatically — allow it to build using
   the plugin whitelist that includes `jekyll-remote-theme` (this happens by default on the
   standard, non-Actions GitHub Pages build).
5. Your site will be live at `https://litonsarker.github.io/` within a few minutes.

## Preview locally (optional but recommended)

```bash
bundle install
bundle exec jekyll serve
```

Then open `http://localhost:4000`.

## Things to personalize before/after publishing

- Add `images/profile.jpg` (your headshot) — referenced in `_config.yml` under `author.avatar`.
- Add project screenshots under `images/portfolio/` — referenced in each `_portfolio/*.md` file.
- Double-check dates/durations on portfolio entries — the original Google Site gave relative
  durations ("3 Years", "6 months") rather than exact dates, so approximate start dates were
  used for sorting purposes only.
- If you'd like a Teaching section or a blog (`_posts/`), the collection is already wired up in
  `_config.yml` for posts; a `_teaching` collection can be added the same way as `_portfolio`
  if you want it later.
- The favorite books/movies section from the old "About me" page was left out as it's not
  typically part of an academic CV site — happy to add it back as a page if you want it.
