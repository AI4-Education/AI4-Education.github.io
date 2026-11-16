# AI4Education — V2 website

A responsive six-page static website, developed from the V1 design and ready for GitHub Pages.

## Pages
- `index.html` — mission, focus areas and audiences
- `research.html` — six substantive research themes and questions
- `projects.html` — six proposed project concepts, steps and intended outcomes
- `team.html` — six role-based capability profiles (not invented personal biographies)
- `activities.html` — five proposed workshop, seminar and community formats
- `contact.html` — collaboration pathways and enquiry guidance

## Publish to GitHub Pages
1. Create a repository named `AI4Education`.
2. Upload the **contents** of this folder to the repository root, including `index.html`, `assets/` and `.nojekyll`.
3. Go to **Settings → Pages → Build and deployment**.
4. Select **Deploy from a branch**, `main`, `/(root)` and save.
5. Visit `https://YOUR-USERNAME.github.io/AI4Education/` after deployment.

## Important before public launch
- Replace capability-based profiles with confirmed names, affiliations, photos and approved biographies.
- Confirm the project status, owners and outputs before calling anything active or completed.
- Add verified activity dates, speakers, venues and registration links when scheduled.
- Add a monitored contact email or integrate a working form service. The current contact page deliberately does not collect messages.
- Check organisational claims, accessibility, privacy, consent and safeguarding requirements.

## Technical notes
Plain HTML, CSS and JavaScript. No backend or build process. Internal links are relative for GitHub Pages project hosting. A future AI platform can add an API/backend, authentication and data handling separately; never expose secret API keys in client-side JavaScript.
