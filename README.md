# Cruise Hub
Save path: C:\MarvelApps\cruisehub\README.md

Live: https://smarvel1963-ops.github.io/cruisehub/ - a Marvel Corp app (Scott 2026-10-04: "build seperate app ...
its independent but also a family of apps").

This repo is Cruise Hub's OWN shell: `index.html`, `manifest.json`, icons and `sw.js` (its own offline worker
and install). The app itself is the shared Hub engine in the Day Hub repo (`../dayhub/features.js`, `app.js`,
`ui.js`, `styles.css`) run with `window.DH_MODE = "cruise"` - one codebase, a fix reaches both apps.

- Own data on the phone (`cruisehub.v1`) and own Google Drive backup (`cruisehub.json`).
- Hub family: shows Day Hub's trips (read only) and Day Hub shows Cruise Hub's - see "hub family" in dayhub/app.js.
- Tests + release steps: the Day Hub repo (`python tests/run_tests.py` covers Cruise Hub too; the test server
  serves C:\MarvelApps so /dayhub/ and /cruisehub/ sit side by side, like on GitHub Pages).
- The old address /dayhub/cruise/ forwards here.
