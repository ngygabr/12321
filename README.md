# 12321

The 12321 board game, live at https://12321.web.app

- `public/index.html` – the game
- `public/lab.html`, `public/lab_hu.html` – tools lab (English / Hungarian)

## Deploying

- Every change merged into `main` is deployed to 12321.web.app automatically
  (`.github/workflows/deploy-live.yml`).
- Every pull request gets a temporary preview link, posted as a comment on the
  pull request (`.github/workflows/deploy-preview.yml`).
- A deploy can also be started by hand: Actions → "Deploy to 12321.web.app" → Run workflow.

The workflows use the repository secret `FIREBASE_SERVICE_ACCOUNT`
(a key for the `github-deploy` service account in Firebase project
`project-523229263760528315`).

The game's source of truth is the "12321" artifact in Claude; the files here are
copies of it.
