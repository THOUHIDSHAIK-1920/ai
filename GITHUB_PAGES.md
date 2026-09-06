# GitHub Pages deployment

This repository is structured with the Vite/React project at the repository root so GitHub Actions can discover `.github/workflows/deploy.yml`.

In GitHub: Settings -> Pages -> Source -> GitHub Actions.

The workflow builds the Vite frontend and publishes `dist/` to GitHub Pages. The Python/FastAPI backend is not hosted by GitHub Pages; backend-dependent API calls need a separately deployed backend.
