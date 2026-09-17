## Summary

<!-- What does this PR change? Keep it short. -->

## Frozen privacy URL (hard checklist)

This URL is a production contract. The App Store listing, the in-app Privacy Policy link, and the marketing site all depend on it remaining **exactly** this path.

**https://devioshdev.github.io/PFRATracker/PrivacyPolicy.html**

- [ ] `PrivacyPolicy.html` **filename is unchanged** (still at repo root; not renamed)
- [ ] `PrivacyPolicy.html` **path is unchanged** (not moved to another folder)
- [ ] Frozen public URL is still exactly `https://devioshdev.github.io/PFRATracker/PrivacyPolicy.html`
- [ ] GitHub Pages project path `/PFRATracker/` is unchanged
- [ ] **Pages smoke check must pass** (do not merge if `.github/workflows/pages-smoke-check.yml` is red, removed, or weakened)

## Do not

- Rename, move, or replace `PrivacyPolicy.html` with a redirect
- Reuse the frozen PFRA policy URL for a different app or page
- Invent unpublished App Store URLs
- Edit the privacy policy body unless the legal content actually needs to change (never as a site reorganization)

New support pages must use **new filenames**.

## Test plan

- [ ] Previewed HTML locally if `index.html` or other public pages changed
- [ ] Pages smoke check GitHub Action is green
- [ ] Confirmed `PrivacyPolicy.html` was not renamed or moved
