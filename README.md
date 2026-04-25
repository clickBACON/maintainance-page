# Maintenance Page (Local Preview)

This folder contains a static `maintenance.html` page. It’s meant to work even if you visit a nested route like `/maintenance/asdd` by using `serve.json` rewrites.

## Prerequisites

- Node.js installed (for `npx`)

## Run locally

From this folder:

```bash
npx --yes serve .
```

It will print a URL like `http://localhost:3000`. Open it in your browser:

- `http://localhost:3000/maintenance.html`
- `http://localhost:3000/maintenance/asdd` (or any other nested path)

## Notes

- `serve.json` is read automatically by `serve` and rewrites `/**` → `/maintenance.html`, so deep links don’t 404.
- If you already have something running on the default port, run:

```bash
npx --yes serve . -l 5050
```

