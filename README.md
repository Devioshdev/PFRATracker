# Deviosh Apps Site

This repository hosts the public support pages for current and future apps by Deviosh.

Live site:
- Site home: `https://devioshdev.github.io/PFRATracker/`
- PFRA Tracker privacy policy: `https://devioshdev.github.io/PFRATracker/PrivacyPolicy.html`

## What's in this repo

- `index.html`: landing page for your app portfolio
- `PrivacyPolicy.html`: current privacy policy linked from PFRA Tracker and store listings
- `.github/workflows/pages-smoke-check.yml`: basic validation so accidental broken deploys are easier to catch
- `.nojekyll`: tells GitHub Pages to serve the site as plain static files

## Safe update workflow

1. Keep `PrivacyPolicy.html` URL and filename unchanged.
2. Add future apps to `index.html` as new public pages go live.
3. Preview the HTML before merging.
4. Merge only after the GitHub Actions check passes.

## Important note

This repository does not contain your mobile app source code. It is the public-facing site layer for app pages, support links, and policy pages.
