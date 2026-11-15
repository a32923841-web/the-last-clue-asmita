# The Last Clue — A 2D Mystery Adventure

A fully offline, self-contained illustrated 2D story made for Asmita. Characters and scenes are drawn locally on Canvas; the portraits, interface, and all sound are local or synthesized in the browser. There are no CDNs, external fonts, online APIs, or remote game assets.

## Play it

1. Extract the ZIP.
2. Start a local server from the extracted project folder: `python -m http.server 8000`
3. Open `http://localhost:8000` in a modern browser.

A hosted first visit needs an internet connection so the browser can download the files and install the service worker. The installed PWA then caches the game for offline play. The game also runs offline from the extracted folder through a local server. Service workers do not work when opening `index.html` directly as a `file://` URL.

## Controls

- Move with WASD or arrow keys. Use the on-screen D-pad on phones.
- Press Space, Enter, or Investigate near a clue.
- Click or tap scene objects to investigate them.
- Use Notebook and Inventory to revisit evidence.
- Escape or Menu opens continue, notes, and restart options.
- Music and sound can be toggled in the top bar.

Progress saves in local storage on the current device and browser. The layout supports portrait and landscape screens, with touch-friendly controls and smooth 2D illustrations.

## The adventure

Explore the moonlit town, a furnished old library with walking and chatting patrons, the park, the station, and the rooftops. Solve five distinct challenges: repeat a streetlamp signal, assemble a torn library message, catch a quick bird, route a train across the signal board, and align a three-symbol lock. Finding all four evidence clues opens a glowing portal that leads into the cave finale.

In the cave, Asmita follows the winding crystal-lit passage to Abhay waiting in silhouette against the sunset. After the letter, they take hands and walk together to a safe inset overlook, then sit side by side while the sunset plays. Asmita’s dark hair, checked detective hat, bright glasses, notebook, and magnifying glass are kept consistent across her smooth animated character and dialogue portrait.

## Project files

- `index.html`, `style.css`, `script.js` — game and responsive interface.
- `manifest.json`, `service-worker.js` — PWA metadata and offline caching.
- `assets/icon.svg` — local install icon.