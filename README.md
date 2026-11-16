# AI4Education website

A responsive, multi-page starter website for AI4Education. Built with plain HTML, CSS and JavaScript so it can be hosted directly on GitHub Pages.

## Pages

- `index.html` — Home
- `research.html` — Research
- `projects.html` — Projects
- `team.html` — Team
- `activities.html` — Activities
- `contact.html` — Contact

## Preview locally

1. Download and extract this project.
2. Open the folder in Visual Studio Code.
3. Open `index.html` in a browser, or use the VS Code Live Server extension.
4. Navigate through all six pages and test the mobile menu.

No build tools, package manager or server are required for the current version.

## Publish with GitHub Pages

1. Create a **public** GitHub repository, for example `AI4Education`.
2. Upload the contents of this folder to the repository root (the `index.html` file must be at the root).
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select branch `main` and folder `/(root)`, then save.
6. Wait for the deployment to finish. Your site will normally be available at:
   `https://YOUR-USERNAME.github.io/AI4Education/`

If you choose a different repository name, the published URL will use that name.

## Before publishing

- Replace `hello@ai4education.example` in `contact.html` and `assets/js/main.js` with a real, monitored email address.
- Replace the sample research themes, project descriptions and team-area descriptions with accurate, approved content.
- Add real team member details and photographs only with their permission.
- Check all links and spelling, and test on desktop, tablet and mobile.
- Consider adding a privacy notice and accessibility statement if you collect personal information or run events.
- The contact form currently uses `mailto:`. It does not submit to a database or send information to a server.

## Designed for future expansion

The project separates page content, styling and shared interactions. This makes it straightforward to add:
- A searchable research and project catalogue.
- Event listings and registration.
- A learning-resource library.
- Student and educator accounts.
- A backend/API layer for AI features.

For future AI integration, keep API keys on a secure server-side backend. Never place private API keys in browser JavaScript or a public GitHub repository. Consider privacy, age-appropriate design, consent, accessibility and human oversight before introducing student-facing AI features.

## Technology

- HTML5
- CSS3 (responsive layout and mobile navigation)
- Vanilla JavaScript
- GitHub Pages-compatible static hosting
