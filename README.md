# PFRATracker — public compliance / support host

**This repository is not the PFRA Tracker app source.**

It is the public GitHub Pages host for Deviosh compliance and support pages (privacy policy, landing, future support URLs). Employers and engineers reviewing this repo should treat it as a frozen static-site contract, not a product codebase.

| What you need | Where it lives |
| --- | --- |
| **This repo** | Public GitHub Pages compliance / support host |
| **Live App Store product** | [PFRA Tracker](https://apps.apple.com/us/app/pfra-tracker/id6762722077) |
| **App source** | Private [`Devioshdev/apps`](https://github.com/Devioshdev/apps) |
| **Marketing site** | [`Devioshdev/deviosh-site`](https://github.com/Devioshdev/deviosh-site) |

## Frozen URL — do not change

This URL is a production contract. The App Store listing, the in-app Privacy Policy link, and the marketing site all depend on it remaining exactly this path:

**https://devioshdev.github.io/PFRATracker/PrivacyPolicy.html**

Do **not**:

- Rename `PrivacyPolicy.html`
- Move it to a different folder or Pages path
- Change the GitHub Pages project URL (`/PFRATracker/`)
- Replace it with a redirect unless every App Store, in-app, and marketing consumer has already been updated (they have not)

Changing this URL will break store compliance links and in-app support.

Live Pages:

- Site home: https://devioshdev.github.io/PFRATracker/
- Frozen privacy policy: https://devioshdev.github.io/PFRATracker/PrivacyPolicy.html

## What's in this repo

- `index.html` — public landing page for the Pages host
- `PrivacyPolicy.html` — PFRA Tracker privacy policy (frozen filename and path)
- `.github/workflows/pages-smoke-check.yml` — GitHub Actions smoke check that required pages exist and key content is present
- `.nojekyll` — tells GitHub Pages to serve the site as plain static files

There is no iOS/Android source, no app build, and no marketing CMS here.

## Safe update workflow

1. Keep `PrivacyPolicy.html` **filename, path, and public URL unchanged**.
2. Prefer README / copy / index updates over policy-path changes. Policy body edits are allowed only when the legal content actually needs to change; never as a way to "reorganize" the site.
3. Add future apps to `index.html` as new public pages go live. New support pages get **new filenames** — do not reuse or relocate the frozen PFRA policy URL.
4. Preview the HTML locally before merging.
5. Merge only after the **Pages smoke check** GitHub Action (`.github/workflows/pages-smoke-check.yml`) passes.

The smoke check verifies that `index.html` and `PrivacyPolicy.html` exist and that key titles/contact content are still present. It does **not** authorize renaming or moving the frozen policy file.
