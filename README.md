# freefield.co

Website for Freefield Labs Inc. and its app, Fairplay – Post Your Plans.

Plain static HTML and CSS. There's no build step, no JavaScript, and no dependencies.

## Pages

| URL | File |
|---|---|
| `/` | `index.html` |
| `/fairplay/support` | `fairplay/support.html` |
| `/fairplay/privacy` | `fairplay/privacy.html` |
| `/fairplay/terms` | `fairplay/terms.html` |
| `/privacy` | `privacy.html` (website privacy notice) |
| 404 | `404.html` |

`vercel.json` turns on clean URLs, so `/fairplay/privacy` serves `fairplay/privacy.html`. It also sets security headers.

## Local preview

```bash
python3 -m http.server 4321
```

Clean URLs only work on Vercel. Locally, open the `.html` paths.

## Deploy

Vercel deploys `main` automatically: no framework preset, no build command, with the repo root as the output directory.

This repository is public. Never commit secrets: `.env*` files, keys and the `.vercel/` folder are git-ignored.
