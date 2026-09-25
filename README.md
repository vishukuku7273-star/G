# CoinLab — iPhone Simple Edition

This folder intentionally contains a single `index.html`. It is easy to upload from an iPhone to GitHub.

## Test on iPhone

1. Create a GitHub repository.
2. Upload `index.html`.
3. Enable GitHub Pages:
   Repository → Settings → Pages → Deploy from branch → `main` → `/root`.
4. Open the generated HTTPS URL in Safari.
5. Share → Add to Home Screen.

## What this version does

- Mobile-first CoinLab UI.
- Trend research interface with clearly-labelled fallback/demo data.
- Idea → ticker concept generation.
- Coin review screen.
- Wallet detection/connect attempt.
- Pump.fun launch UI placeholder.

## Why the real launch backend is separate

X bearer tokens and transaction-building credentials must not be placed in browser code. A production version should use a server/API route for:
- live X search
- AI clustering
- metadata upload
- Pump.fun transaction construction
- rate limiting and validation

The user's wallet should sign the resulting transaction in the browser/wallet. Never collect seed phrases or private keys.
