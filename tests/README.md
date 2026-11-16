# Portfolio regression checks

Serve the repository over HTTP on localhost, open `/tests/portfolio.html`, and click **Run local checks**. No package installation is required; the app's existing CDN dependencies must be available.

The checks exercise the real app in an iframe: cover and profile fields, safe documentation links and QR, goal heading placement, sidebar logo, widths 320/390/768/1280, a generated two-page PDF upload, single-sheet and four-item grid layouts, image resolution, print boundaries, original-file persistence, and a full portfolio export with a clickable URL and matching page geometry.

Use a separate browser profile or port with disposable local data. Tests temporarily replace the local state and restore the previous state in `finally`. They cannot run on the production hostname. Nothing contacts or modifies production storage.
