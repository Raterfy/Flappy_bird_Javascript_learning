# Flappy Bird — JavaScript learning project

This repository contains a simple Flappy Bird implementation in JavaScript, created as a learning project to teach DOM manipulation, basic animation, input handling, and client-side game logic.

## Overview
A small reflex game where the player keeps the bird in the air to pass between columns.

- Languages: HTML, CSS, JavaScript
- Main game folder: `flappy_bird/`
- Key files:
  - `flappy_bird/index.html` — main HTML page
  - `flappy_bird/app.js` — game logic (engine, collisions, input)
  - `flappy_bird/assets/` — images, sounds and other resources

## How to run (locally)
The game is a static web app; no dependencies are required.

1. Open `flappy_bird/index.html` directly in a modern browser (Chrome, Firefox, Edge).
2. (Optional) Serve the folder locally to avoid resource-loading issues with the `file://` protocol:

   - With Python 3:

```bash
cd flappy_bird
python3 -m http.server 8000
# then open http://localhost:8000 in your browser
```

   - With Node (if installed):

```bash
# install http-server if needed
npm install -g http-server
cd flappy_bird
http-server -c-1
# open the URL shown (e.g. http://127.0.0.1:8080)
```

## Controls
- Space: start the game
- Up Arrow: make the bird jump (flap)

## Project structure
```
Flappy_bird_Javascript_learning/
├─ __MACOSX/            # system archive (can be ignored)
├─ flappy_bird/
│  ├─ index.html
│  ├─ app.js
  │  └─ assets/           # images, sounds, etc.
└─ README.md
```

## Quick customization
- Change pipe speed: edit the speed constants in `flappy_bird/app.js`.
- Replace sprites or sounds: swap files in `flappy_bird/assets/` (keep file names if referenced directly).
- Adjust physics (gravity, jump power): look for `gravity`, `jump`, `velocity` or similar variables in `app.js`.

## Development tips
- Open the dev console (F12) to see JavaScript errors.
- If assets don't update, try clearing the browser cache or use a hard reload.
- Commit small, focused changes with clear messages.

## Quick tests
- Confirm the page loads without console errors.
- Press Space to start, then Up Arrow to make the bird jump.
- Collide the bird with a column or the ground to check collision detection and game over behavior.

## Known issues & troubleshooting
- If images/sounds fail to load when opening the file directly (`file://`), run a local server (see instructions above).
- If the game doesn't respond to input, ensure `app.js` is included in `index.html` and check the console for errors.

## Contributing
Contributions are welcome — bug fixes, improvements, and new features.

- Fork the repo
- Make changes in a feature branch
- Open a Pull Request describing your changes

## Credits
Personal learning project. Inspired by the original Flappy Bird by Dong Nguyen.