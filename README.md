# AI4Education

A responsive six-page educational website using plain HTML, CSS and JavaScript. No build tools or dependencies required. Open `dist/index.html` locally or serve `dist/` with any static web server.

## Project structure

- `dist/index.html`: Home
- `dist/research.html`: Research agenda
- `dist/projects.html`: Grant-funded workshops, project listing and roadmap
- `dist/team.html`: Eight team members with Griffith profile photos and links
- `dist/activities.html`: Educator roundtable, school workshops, GRAIL and school engagement
- `dist/contact.html`: Locally downloadable enquiry (no transmission)
- `dist/assets/`: Shared stylesheet, JavaScript and favicon
- `docs/ARCHITECTURE.md`: Extension and service integration guidance
- `.github/workflows/pages.yml`: GitHub Pages deployment

## Upload to GitHub

1. Create an empty GitHub repository.
2. Upload this entire project folder, including `.github` (or use Git commands below).
3. In Settings → Pages → Build and deployment, select **GitHub Actions**.
4. Push to `main`. The included workflow deploys only `dist/`.
5. Open the Pages URL shown by GitHub when the workflow succeeds.

```sh
git init
git add .
git commit -m "Create AI4Education website"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/AI4Education.git
git push -u origin main
```

All internal links and assets use relative paths, supporting repository subpaths on GitHub Pages. This package excludes Sites hosting metadata and Git history; it is ready for an independent GitHub repository.

## Editing

Edit each page's semantic HTML. Shared header/footer markup is repeated to keep every page complete without JavaScript; update it across all six pages when changing navigation. Styles use shared tokens in `:root`; interactions are progressively enhanced in `main.js`. Google Fonts are optional: system fonts work without network access.

## Current content and functionality

This package includes the latest website updates as of 16 November 2026: Griffith branding and campus photograph; the grant-funded cyber risk workshops; eight team members; educator discussions, Somerset and Helensvale workshops; GRAIL and school engagement; and training opportunities on Contact.

The second project is marked “details to be announced”. The Contact form downloads an enquiry text file; it does not send email or submit to a server. AI services, accounts and progress tracking are future extensions, described in `docs/ARCHITECTURE.md`.

Photos, the university logo and their source records are bundled in the package. Institutional imagery retains its original ownership; no blanket open-source licence is applied to these assets.

## Quick local preview

Open `dist/index.html`, or run:

```sh
python -m http.server 8000 --directory dist
```

Then visit http://localhost:8000.

## Important upload detail

Extract the ZIP first. Upload the contents of the inner `AI4Education` folder to the repository root: `dist`, `docs`, `.github`, `README.md` and `.gitignore`. Do not upload the ZIP itself or nest the project under another folder. Make sure the `.github/workflows/pages.yml` file is included. Select **GitHub Actions** in repository Settings → Pages before running the deployment workflow.
