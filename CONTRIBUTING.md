# Contributing

## Branches

- `main` is always working. Nothing goes in directly.
- Build each feature on its own branch, named `<area>/<short-name>`, for example:
  - `firmware/sensor-read`
  - `backend/firebase-api`
  - `ml/data-cleaning`
  - `app/result-screen`
  - `docs/fmea`
- Keep a branch focused on one feature and short-lived.

## Workflow

1. `git checkout main && git pull`
2. `git checkout -b ml/data-cleaning`
3. Commit small, with clear messages ("ml: drop duplicate rows").
4. Push and open a pull request into `main`.
5. Review it (a teammate if possible), then merge. Delete the branch.
6. Before the final integration, pull `main` into your branch and check everything still runs.

## Rules

- No secrets in git: Firebase keys, WiFi passwords, `google-services.json`, `.env`. They are in `.gitignore`.
- Do not commit raw datasets with personal or health information. Describe them in `data/README.md` instead.
- Split train/test by participant or source before any preprocessing.
- Label results from public or simulated data as such.
- No clinical claims in code comments, docs, or the app.
