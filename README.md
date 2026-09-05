# FPL Manager — iPhone/GitHub Pages build

This build fixes the browser CORS problem by reading `data/fpl.json` from the same GitHub Pages site. A GitHub Action fetches the public FPL API and refreshes the cache automatically.

## Install
1. Put these files in the root of your GitHub Pages repository: `index.html`, `model.js`, `manifest.webmanifest`.
2. Create `.github/workflows/update-fpl-data.yml` using the supplied workflow.
3. Wait for the workflow to complete. It creates `data/fpl.json`.
4. Open the GitHub Pages site in Safari and tap Refresh.
5. Safari → Share → Add to Home Screen → Open as Web App → Add.

The app does not ask for an FPL password. The public FPL API is used only by the server-side GitHub Action, not directly by Safari.
