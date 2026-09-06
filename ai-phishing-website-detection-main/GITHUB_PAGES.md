# GitHub Pages deployment

This repository is configured for GitHub Pages static hosting.

- The Vite app uses relative asset paths (`base: './'`).
- The entry script is relative so it works at `/REPOSITORY_NAME/`.
- GitHub Pages runs the frontend only; the Express/Python backend is not deployed there.
- `src/services/api.ts` falls back to the browser-side URL classifier when `/api/predict` is unavailable.

Enable **Settings → Pages → Source: GitHub Actions**, then push to `main`.
