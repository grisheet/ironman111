# Holographic Command Interface

Single-file, no-build app. Gesture-controlled hologram using your webcam.

## Deploy on GitHub Pages
1. Put these files in the root of your repo (branch `main`). Remove any old files (src, package.json, .github).
2. Settings -> Pages -> Source: "Deploy from a branch" -> `main` / `(root)` -> Save.
3. Open https://<user>.github.io/<repo>/ after ~1 minute and hard-refresh.

## Run locally
    python3 -m http.server 8000      # then open http://localhost:8000
(Webcam needs HTTPS or localhost; opening the file directly will not work.)

## Controls
Point = cursor | Pinch over core = grab | Two hands pinching on core = scale + twist
Mouse: drag + wheel | Keys: R reset, 1/2/3 forms

## Notes
- Three.js and MediaPipe load from the jsDelivr CDN; the hand model downloads from Google storage on first Start. Internet required.
- No video is recorded or uploaded; inference runs in your browser.
