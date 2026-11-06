# S-Coding Studio

Phone-friendly web code editor: HTML, CSS, JS, JSON, TS, TSX, Python, ZIP website preview and an AI bug-fix assistant.

## GitHub Pages par chalane ke steps
1. GitHub par naya repo banao (Public) aur in sab files ko upload karo (`index.html`, `sw.js`, `manifest.json`, `icon-192.png`, `icon-512.png`, `apple-touch-icon.png`).
2. Repo mein **Settings -> Pages -> Build and deployment** -> Source: *Deploy from a branch* -> Branch: `main` / `(root)` -> Save.
3. 1-2 minute baad app yahan khulega: `https://USERNAME.github.io/REPO-NAME/`
4. Phone ke Chrome mein is link ko kholo -> menu -> **Install app / Add to Home screen**.

## Zaroori baatein
- **API key kabhi code ya repo mein mat likho.** App mein koi key nahi hai; jo key aap settings mein daalte ho woh sirf aapke apne browser mein save hoti hai.
- Update karne par `sw.js` mein `scs-v5` ko `scs-v6` karo, tab purana cached version hat jayega.
- Python (Pyodide), TS/TSX (Babel) aur fonts internet se aate hain; pehli baar chalane ke baad browser unhe cache kar leta hai.
