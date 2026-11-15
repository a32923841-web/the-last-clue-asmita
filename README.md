# The Last Clue — A 2D Mystery Adventure

A fully offline, self-contained illustrated 2D story made for Asmita. Characters and scenes are drawn locally on Canvas; the portraits, interface, and all sound are local or synthesized in the browser. There are no CDNs, external fonts, online APIs, or remote game assets.

## Play it

1. Extract the ZIP.
2. Start a local server from the extracted project folder: `python -m http.server 8000`
3. Open `http://localhost:8000` in a modern browser.

A hosted first visit needs an internet connection so the browser can download the files and install the service worker. The installed PWA then caches the game for offline play. The game also runs offline from the extracted folder through a local server. Service workers do not work when opening `index.html` directly as a `file://` URL.

## Controls

- Move with WASD or arrow keys. Hold Shift to run. Use the on-screen D-pad on phones.
- Press Space or Up to jump and dodge; press E or Enter near a clue or character.
- Press J or the on-screen ACT button during the rooftop spar to strike. Jump over the keeper’s wind-up swing.
- Space or Enter advances dialogue; tap the dialogue panel or arrow to continue.
- Click or tap scene objects to investigate them.
- Use Notebook and Inventory to revisit evidence.
- Escape or Menu opens continue, notes, and restart options.
- Music and sound can be toggled in the top bar.

Progress saves in local storage on the current device and browser. The title screen offers a clear **Continue Investigation** option whenever a case is saved; starting a new case asks before replacing that save. The layout supports portrait and landscape screens, with touch-friendly controls and smooth 2D illustrations.

## The adventure

Run, jump, and explore a continuous side-scrolling route through the moonlit town, a furnished old library with walking and chatting patrons, the park, the station, and the rooftops. Solve the streetlamp signal, rebuild a library cipher, reach the raised photo trail, route a train, win a live rooftop spar, and open the safe. Finding all four evidence clues opens a glowing portal into the cave finale.

In the cave, a slow camera move reveals Abhay waiting just inside the exit, silhouetted against a sunset framed by the cave mouth. After the letter, he takes Asmita’s hand and they walk together to a safe inset overlook, then sit side by side while the sunset plays. Asmita’s dark hair, detective hat, clearly visible glasses, notebook, and magnifying glass stay consistent in the game and dialogue portrait.

## Project files

- `index.html`, `style.css`, `script.js` — game and responsive interface.
- `manifest.json`, `service-worker.js` — PWA metadata and offline caching.
- `assets/icon.svg` — local install icon.
