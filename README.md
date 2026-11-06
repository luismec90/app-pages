# App Pages

The privacy policies and support pages of my iPhone apps. GitHub Pages serves this repository's `main` branch at
https://luismec90.github.io/app-pages/.

## How it's laid out
- One folder per app, named as in its addresses. Each holds four pages, in English and Spanish: `privacy.en.html`,
  `privacy.es.html`, `support.en.html` and `support.es.html`. The app opens them from About (its `AppLinks.swift`),
  and App Store Connect lists them as the Privacy Policy and Support URLs, so a page's name never changes.
- `unclog/`: Unclog's pages until 6 November 2026, when they moved to the app's own site, getunclog.app (`website/`
  in its repository). Builds up to 1.0 (2) still open them from About, so the folder stays, unchanged.
- `freemystorage/`: Unclog's pages from when it was called FreeMyStorage, free with no purchase. Its first TestFlight
  builds still link there, so the folder stays, unlisted and unchanged.
- `style.css`: the look of every page, in light and dark mode. The pages load nothing from other sites: no fonts,
  scripts, cookies or analytics, as their privacy policies say.
- `index.html`: links to each app's pages.
- `.nojekyll`: GitHub Pages publishes the files as they are, without building them with Jekyll.

## Changing a page
Change the English and Spanish pages together, and the date under a privacy policy's title. A push to `main`
publishes in a minute or two; the repository's Actions tab shows the "pages build and deployment" run.

## Adding an app
Copy an app's folder, name it as in the new app's `AppLinks.swift`, rewrite the four pages from what the new app does,
and link them from `index.html`.
