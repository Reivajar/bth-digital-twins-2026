# Digital twins for urban planning, BTH

Course site for the one-week module (9–13 November 2026), plus the student starter kit. Static files only, no build step.

## What is in this repository

| Path | What it is |
| --- | --- |
| `index.html` | The course page |
| `assets/remixicon/` | Icon font used by the page. Keep it next to `index.html` |
| `files/` | Everything listed in the page's Documents section. Subfolders become headings |
| `files/starter-kit/helsingborg-starter-kit.zip` | The kit students download |
| `files/templates/` | Requirement brief template |
| `starter-kit/` | The kit's source, unzipped. Also works as a hosted viewer at `<site>/starter-kit/` |
| `.nojekyll` | Tells GitHub Pages to serve files as they are |

## Publish (once)

1. On github.com, create a **public** repository, for example `bth-digital-twins`. (Private repos only get Pages on a paid plan.)
2. Upload everything in this folder, including `.nojekyll`, `.gitignore` and the `files/` folder. Or from a terminal in this folder:
   ```
   git init -b main
   git add .
   git commit -m "Course site and starter kit"
   git remote add origin https://github.com/<your-username>/bth-digital-twins.git
   git push -u origin main
   ```
3. Settings → Pages → Source: *Deploy from a branch*, branch `main`, folder `/ (root)`.
4. After a minute the site is at `https://<your-username>.github.io/bth-digital-twins/`.

The Documents list reads this repository through the GitHub API (branch `main`, folder `files/`). If the branch or repo name differs, set `REPO` and `BRANCH` in the script at the bottom of `index.html`.

## Add a document

On github.com open `files/` (or a subfolder such as `files/slides/`) → **Add file → Upload files** → **Commit changes**. It shows up in Documents within a minute or two.

Only you and collaborators can upload. Hand-ins go through BTH's learning platform.

## Change the starter kit

Edit the files in `starter-kit/`, then zip the folder again and replace `files/starter-kit/helsingborg-starter-kit.zip`. The zip must contain one folder named `helsingborg-starter-kit`.

## Edit the page

Everything is in `index.html`. Unsettled items are marked `<span class="tbc">…TBC</span>`; search for `tbc`.

## What never goes in this repository

- Paywalled PDFs. Link the DOI; only open-access PDFs go in `files/readings/`.
- Student names, group lists with names, questionnaire answers.
- Teacher-only notes: the project's `docs/`, `teacher/` and `PROJECT-CONTEXT.md`.
- The city's SketchUp/OBJ model files (large, and the licence is not stated).

## Data and licences

Starter-kit data: Overture Maps Foundation (includes OpenStreetMap contributors and Microsoft ML Buildings, ODbL) and Copernicus DEM GLO-30. MapLibre GL JS is BSD-3-Clause (`starter-kit/lib/MAPLIBRE-LICENSE.txt`). Remix Icon: see `assets/remixicon/License`. Details in `starter-kit/docs/DATA.md`.
