# skaglobal.github.io redirect

This tiny user-site redirects visitors from the root user site to the project site at `/my_cards/`, preserving query parameters and hash fragments.

## How to set up

1) Create a new public repo named exactly:

   skaglobal/skaglobal.github.io

2) Copy these files into the repo (or upload the provided ZIP):

- `index.html` — immediate redirect to `https://skaglobal.github.io/my_cards/`
- `404.html` — fallback redirect for unknown paths

3) Enable GitHub Pages for the repo:

- Settings → Pages → Build and deployment → Source: **Deploy from a branch**
- Branch: **main**, Folder: **/** (root)

GitHub Pages will deploy in under a minute. Visiting `https://skaglobal.github.io` will then forward to `https://skaglobal.github.io/my_cards/`.

### Optional
- If you later add a custom domain, this redirect still works.
- You don’t need Jekyll or any workflow—this is static HTML+JS.
