# App-Details

This repository hosts the static legal pages for the **Fitness Trackfit** mobile app:

- `FitnessTrackfit/privacy-policy.html`
- `FitnessTrackfit/terms-and-conditions.html`

These are the store-listing / in-app "legal" pages. The mobile app's source code lives in a separate repository and is **not** part of this repo.

## Cursor Cloud specific instructions

- This is a **static-content-only** repo: two self-contained HTML files (inline CSS, no JS, no external assets) plus this README/AGENTS. There is **no** package manager, build system, test suite, backend, or database, so there is nothing to install, build, or lint.
- To preview/serve the pages during development, run a static file server from the repo root and open the files in a browser:
  - `python3 -m http.server 8000` (from `/workspace`)
  - Pages: `http://localhost:8000/FitnessTrackfit/privacy-policy.html` and `http://localhost:8000/FitnessTrackfit/terms-and-conditions.html`
  - The port is not fixed by anything in the repo; any static server/port works.
- Edits to the HTML are picked up on a normal browser refresh (the static server does not cache); no restart needed.
