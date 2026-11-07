# S-Coding Studio

Phone-friendly web code editor: HTML, CSS, JS, JSON, TXT, TS, TSX, Python, ZIP website preview and an AI bug-fix assistant.

## GitHub Pages par chalane ke steps
1. GitHub par naya repo banao (Public) aur in sab files ko upload karo (`index.html`, `sw.js`, `manifest.json`, `icon-192.png`, `icon-512.png`, `apple-touch-icon.png`).
2. Repo mein **Settings -> Pages -> Build and deployment** -> Source: *Deploy from a branch* -> Branch: `main` / `(root)` -> Save.
3. 1-2 minute baad app yahan khulega: `https://USERNAME.github.io/REPO-NAME/`
4. Phone ke Chrome mein is link ko kholo -> menu -> **Install app / Add to Home screen**.

## Zaroori baatein
- **API key kabhi code ya repo mein mat likho.** App mein koi key nahi hai; jo key aap settings mein daalte ho woh sirf aapke apne browser mein save hoti hai.
- Har update par `sw.js` ka cache version badhao (is build mein `scs-v11`; agla `scs-v12`), tab phone par purana cached version hat jayega.
- Python (Pyodide), TS/TSX (Babel) aur fonts internet se aate hain; pehli baar chalane ke baad browser unhe cache kar leta hai.

## Features (tools menu `⋯` editor ke upar)
- **Ek preview:** HTML + CSS + JS + JSON + TXT + TS + TSX + Python aur (+) se bane saare tabs ek hi preview mein judte hain.
- **Project ZIP export/import:** har tab apne file naam se (folder ke liye tab ka naam `lib/utils.js` rakho). Import mein `studio.json` se sab kuch wapas.
- **Auto-backup:** har save ke baad IndexedDB mein doosri copy; browser ka data saaf ho jaye to project wapas aa jata hai.
- **Find / Replace:** is tab mein ya sab tabs mein.
- **Autocomplete:** typing par suggestions (keywords + sab tabs ke words).
- **Error check:** JS, JSON, CSS, HTML, Python, TS mein galti ki line gutter mein laal; upar `✖ N` dabao.
- **Tabs ke beech import:** `import {add} from './utils.js'` (JS tabs, JSON tabs, folder naam). Bare naam (`import _ from 'lodash'`) npm package `esm.sh` se aata hai (internet chahiye).
- **Python:** preview page ke andar chalta hai (`from js import document` se page chhu sakte ho). Python tabs ek doosre ko `import helper` se import kar sakte hain.
- **Code format:** Prettier (internet se, pehli baar).
