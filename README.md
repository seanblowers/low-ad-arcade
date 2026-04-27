# Low-Ad Arcade

A small collection of custom-built browser games. No ads, no tracking, no
sign-ups, no microtransactions. Just little hand-made things to play with for
five minutes between meetings.

## Playing

Open `index.html` in a browser, or serve the folder with anything that hands
back static files:

```sh
python3 -m http.server 8000
# then visit http://localhost:8000
```

Each game is a single self-contained HTML file under `games/<name>/index.html`.
No build step, no bundler, no framework.

## Games

| Game | Path | What it is |
| --- | --- | --- |
| 🐰 Bunny Clicker | `games/bunny-clicker/` | Cookie-clicker-style idle game |
| 🫧 Bubble Wrap | `games/bubble-wrap/` | Pop bubbles. Refill. Repeat. |

## Adding a new game

1. Create `games/<your-game>/index.html`. Make it standalone.
2. Add a card to the grid in the root `index.html` (look for `GAMES`).
3. That's it.

Convention: every game's top-left should have a small "← arcade" link back to
the root, so players can hop between them without using the back button.

## Why "low-ad"

Casual web games used to be a delight. Then ads ate them — interstitials, popups,
"watch a 30-second video to continue," cookie banners stacked on cookie banners.
This is the opposite of that.
