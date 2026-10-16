# harisaran.dev

Personal landing page. One static file, no build step.

- `index.html` — the whole site: markup, styles, script, and the fonts embedded as woff2
- English / French, switched client-side and remembered in `localStorage`
- No external requests at runtime

## Run locally

```sh
python3 -m http.server 8000
```

## Deploy

GitHub Pages serves `main` from the repository root, so a push deploys.

- `CNAME` holds the custom domain, `harisaran.dev`
- `.nojekyll` turns off Jekyll, which has nothing to do here
- DNS lives at Cloudflare: four A and four AAAA records at the apex pointing to
  GitHub Pages, plus `www` as a CNAME. Keep them unproxied (grey cloud), or
  GitHub cannot renew the TLS certificate.
