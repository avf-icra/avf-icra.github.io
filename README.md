# avf-website (anonymized)

Project page for **Active Visual Fixation (AVF)**. Static site (no build step). This is a scrubbed,
anonymized copy prepared for double-blind review — see NOTES-ANON.md for what was changed.

## Files

| File | Purpose |
|------|---------|
| `index.html` | The whole page. |
| `style.css` | Design system. |
| `script.js` | Legacy object-viewer helpers (mostly unused; live carousels are inline in `index.html`). |
| `data/` | All media (videos, figures, favicon, preview card). |
| `viewer/` | Interactive avf-eval viewer, vendored as plain files (not a submodule) for anonymity. Served at `/viewer`. |

## Local preview

```bash
python -m http.server 8000
```

Then open <http://localhost:8000>.

## Deploying (GitHub Pages)

1. Push to a GitHub repo under the anonymous account.
2. Repo **Settings → Pages → Build from branch**, pick the branch + `/ (root)`.
3. No custom domain / CNAME — keep it on the default `*.github.io` URL.
