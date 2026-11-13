# okashaluai.github.io

Personal site of Luai Okasha, built with [Hugo](https://gohugo.io) (extended, v0.139+). English at `/`, German at `/de/`.

## Run locally

```sh
hugo server -D      # -D also shows drafts
```

## Where things live

| What | File |
|---|---|
| Disclosures table (home + Advisories) | `data/advisories.yaml` |
| Project cards | `data/projects.yaml` |
| "now" box on the home page | `data/now.yaml` |
| Home "Selected work" cards | `content/_index.en.md`, `content/_index.de.md` |
| Email, GitHub, LinkedIn, PGP, CV links | `[params]` in `hugo.toml` |
| UI text in both languages | `i18n/en.yaml`, `i18n/de.yaml` |
| Styles | `static/css/site.css` |
| security.txt (renew `Expires` yearly) | `static/.well-known/security.txt` |

## Write a new writeup

```sh
hugo new writeups/my-post/index.en.md
```

Fill in the front matter (`tldr`, `summary_de`, optional `advisory` and `timeline`), write the post, then set `draft: false`.
Use `{{</* callout */>}}…{{</* /callout */>}}` for a highlighted note.
Writeups are English-only; the German summary box comes from `summary_de`.

## Before going live

- [ ] Fill `severity`, `date` (and `writeup` once published) in `data/advisories.yaml`
- [ ] Check the GHSA and repo URLs in `data/advisories.yaml` and `data/projects.yaml`
- [ ] Add your LinkedIn URL to `hugo.toml`
- [ ] Put corrected CV PDFs in `static/cv/` and set `cvEN` / `cvDE`
- [ ] Optional: export your PGP public key to `static/pgp.asc`, set `pgpFingerprint`, and add the `Encryption:` line to security.txt
- [ ] Have someone check the German texts

## Deploy

GitHub → **Settings → Pages → Build and deployment → Source: GitHub Actions**.
Every push to `main` builds and deploys with `.github/workflows/hugo.yml`.

Fonts (Inter, Space Grotesk, JetBrains Mono, SIL OFL) are self-hosted in `static/fonts/` so the site makes no third-party requests.
