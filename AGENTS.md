## Cursor Cloud specific instructions

This is a **purely static HTML/CSS website** (personal portfolio / GitHub Pages site). There is no build system, no package manager, no backend, and no dependencies to install.

### Serving locally

Use any static file server. The `.vscode/settings.json` configures VS Code Live Server on port **5501**. In headless/cloud environments, use:

```
npx serve -l 5501 /workspace
```

### Project structure

- `/index.html` — Main homepage
- `/resume/` — Resume page
- `/subpages/happy-birthday/` — Birthday invitation page
- `/subpages/Monthly_Resolution/` — Monthly resolutions blog
- `/subpages/Blogs/` — Blog index pages (Physics & CS)
- `/testthreejs/` — Pre-bundled Three.js demo
- `/css/` — Shared stylesheets
- `/images/` — Shared images
- `/ssl/` — SSL certificates for domain hosting

### Notes

- No lint, test, or build commands exist — there are no `package.json`, `Makefile`, or CI configs.
- The `CNAME` file maps to `zxzq.me` for GitHub Pages deployment.
- External fonts and icons are loaded from CDNs (Google Fonts, staticfile.org); pages need internet access to render fully.
