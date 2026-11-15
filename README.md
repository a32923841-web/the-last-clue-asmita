# The Last Clue — A Pixel Story for Asmita

A responsive, offline-first pixel-art detective game made for Asmita, by Abhay. All scenes and character sprites are drawn locally in Canvas; sound effects and ambient music are synthesized in the browser. The project has no CDN, online API, remote fonts, or external game assets.

## Play it

1. Extract the ZIP.
2. Open a terminal in the extracted `the-last-clue` folder.
3. Start a local server with Python: `python -m http.server 8000`
4. Open `http://localhost:8000` in Chrome, Edge, or Firefox.

The first visit should be online if you want the browser to install the service worker and cache the complete game. After that, the installed PWA can open offline. You can also keep the extracted folder and run the local server without internet. Service workers do not work when opening `index.html` directly as a `file://` URL.

## Controls

- Move with WASD or arrow keys; on phones, use the on-screen D-pad.
- Press Space, Enter, or the Investigate button near a clue.
- Click or tap scene objects to investigate them directly.
- Use Notebook and Inventory to revisit collected evidence.
- Escape or Menu opens continue, notebook, and restart options.
- Music and sound toggles are in the top bar.

Progress is saved in local storage on the current device/browser. Restart clears the saved case. Layout supports portrait and landscape screens; pixel graphics use crisp nearest-neighbour scaling.

## Project files

- `index.html`, `style.css`, `script.js` — game and responsive interface.
- `manifest.json`, `service-worker.js` — PWA metadata and offline caching.
- `assets/icon.svg` — local install icon.

## Scenes and story

Explore the moonlit town, a fully furnished old library with browsing and chatting patrons, the quiet park, old station, and rooftop. Solve five short mini-games (lantern sequence, library book order, park memory trail, station signals, and rooftop lock) to earn clues. Chapter transitions use cinematic story beats and moving scene details. Then follow the winding cave passage to Abhay waiting in silhouette at the sunset opening. After the letter, take his hand and walk together to a safe inset overlook, then sit side by side as the sunset plays. Asmita's detective hat, dark hair, notebook, magnifying glass, and clearly visible spectacles stay consistent in her world sprite and dialogue portrait.
