# Burst – Cracker Photo Studio

Take a live camera view or a photo, choose crackers, tap to burst them, then record a video or take a screenshot. Works offline once installed.

## Features
- **Live camera or photo:** front/back camera, take photo, or upload.
- **Sky crackers:** Chrysanthemum, Peony, Willow, Palm, Ring, Heart, Crossette, Crackle, Rocket, Sky shot, Comet.
- **Ground crackers:** Fountain, Chakra, Flowerpot, Sparkler, Bijili, Atom bomb, Snake.
- **Fuse lighting:** a wick burns before each cracker goes off (can be turned off).
- **Sound:** synthesized boom, whistle and crackle.
- **Controls:** colour palettes, size, night level, Grand finale.
- **Capture:** on-screen Screenshot and Record buttons (video with sound).
- **Installable and offline:** PWA with a service worker.

Everything runs in the browser. Photos and videos never leave your device.

## Run locally
Serve the folder over HTTPS or localhost (camera needs a secure origin):

    python3 -m http.server 8000

Open http://localhost:8000

## Deploy to GitHub Pages
1. Install the GitHub CLI and run `./deploy.sh` (optionally `./deploy.sh my-repo-name`).
2. Or push to a repo and set Settings > Pages > Source to GitHub Actions. The workflow in `.github/workflows/pages.yml` publishes on every push to `main`.

## Files
- `index.html`: the whole app
- `sw.js`, `manifest.json`, `icon-*.png`: offline and install support
- `deploy.sh`: creates the repo, pushes and enables Pages

## License
MIT
