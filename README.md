# PFRA Tracker Site

This repository hosts the public support pages for the PFRA Tracker app.

Live site:
- Privacy policy: `https://joshsaez.github.io/PFRATracker/PrivacyPolicy.html`
- Project page: `https://joshsaez.github.io/PFRATracker/`

## What's in this repo

- `index.html`: lightweight landing page for the app's public web presence
- `PrivacyPolicy.html`: privacy policy linked from the app and store listings
- `.github/workflows/pages-smoke-check.yml`: basic validation so accidental broken deploys are easier to catch
- `.nojekyll`: tells GitHub Pages to serve the site as plain static files

## Safe update workflow

1. Keep `PrivacyPolicy.html` URL and filename unchanged.
2. Make content changes in a branch first.
3. Preview the HTML before merging.
4. Merge only after the GitHub Actions check passes.

## Important note

This repository does not contain the mobile app source code. It is only for the public-facing website and policy pages used by the deployed app.
