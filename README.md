# Farhan Ellahi — Portfolio

Static portfolio for GitHub Pages. All content lives in `data.json`; `index.html` only renders it.

## Edit content

Open `data.json` and change the text. Commit, and GitHub Pages updates in about a minute.

- **Section order / hide a section:** edit the `order` list. Remove a name to hide that section.
- **Stats:** `stats` list (`value` and `label`).
- **Add a job:** copy an item inside `experience.items`. Newest first.
- **Add a project:** copy an item inside `projects.items`. Set `"featured": true` for a full-width card.
- **Education / certifications:** `education.items` and `education.certifications.items`.
- **Contact:** `contact.items` and `contact.buttons`.

## Add pictures

1. Put the image in the `assets/` folder, for example `assets/writon.png`.
2. In `data.json` set `"image": "assets/writon.png"` on the project.

The same works for `"logo"` on a job and `"photo"` in `hero`. Leave the value empty (`""`) to show nothing.
Use 1600×900 (16:9) images, under 300 KB each.

## Deploy

Repo Settings → Pages → Deploy from a branch → `main` / `/ (root)`.

Site URL: `https://thenanosoft.github.io/<repo-name>/`

To test locally run `python -m http.server` in this folder and open `http://localhost:8000`.
Double-clicking `index.html` will not work because browsers block loading `data.json` from a file.
