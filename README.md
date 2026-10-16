# harisaran.dev

Personal landing page. One static file, no build step.

- `index.html` — the whole site: markup, styles, script, and the fonts embedded as woff2
- English / French, switched client-side and remembered in localStorage
- No external requests at runtime

## Run locally

```sh
python3 -m http.server 8000
```

## Deploy

Serve the folder as static files. Nothing to compile.
