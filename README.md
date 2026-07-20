# RentalMate — Legal pages

Public pages for App Store compliance (Privacy Policy, Terms of Use, Support).

## Live URLs (GitHub Pages)

- https://linhlm310.github.io/rental-mate-legal/
- https://linhlm310.github.io/rental-mate-legal/privacy.html
- https://linhlm310.github.io/rental-mate-legal/terms.html
- https://linhlm310.github.io/rental-mate-legal/support.html

Deploy source: branch **`gh-pages`** (root). Keep `main` in sync for editing.

## Edit workflow

1. Edit HTML on `main` (or copy from private app repo `docs/legal/`).
2. Publish to Pages:

```bash
git checkout gh-pages
git checkout main -- index.html privacy.html terms.html support.html
touch .nojekyll
git add -A && git commit -m "Update legal pages"
git push origin gh-pages
git checkout main
```

3. Wait for Pages build (Settings → Pages). If stuck on “errored”, open Settings → Pages and click **Save** once.

App constants: `lib/core/constants/legal_urls.dart` in the private RentalMate repo.
