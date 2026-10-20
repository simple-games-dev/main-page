# 🎲 Simple Games

Board games you can play in your browser — no installs, no sign-ups. Make a room, send the code to a friend, and play. Or just pass one device around the table.

**▶ Play:** https://simple-games-dev.github.io/main-page/

---

## The games

| | Game | Players | What's it about? |
|---|---|---|---|
| 💎 | **[Gem Merchants](https://simple-games-dev.github.io/merchants/)** *(new)* | 2–4 | Collect gems, buy cards that make your next purchases cheaper, and attract nobles. First to 15 prestige triggers the final round. |
| 🗼 | **[Ascent](https://simple-games-dev.github.io/ascent-game/)** | 2–3 | Climb three storeys or be the last builder standing. Move, build, and out-think your rivals on a 3D tower board. |
| 🌿 | **[Hedgerow](https://simple-games-dev.github.io/hedgerow/)** | 2–4 | Race your pawn across the garden — or drag hedges onto the board to slow everyone else down. You can never trap a player completely. |
| 👻 | **[Ghosts](https://simple-games-dev.github.io/ghosts/)** | 2 | Each side has good and poisoned ghosts, and only you know which is which. Capture the wrong one and you lose your own. Get a good ghost across to win. |
| 🏝️ | **[Colonist](https://simple-games-dev.github.io/colonist/)** | 2–4 | Settle the island, trade with friends, build roads and cities, and race to 10 points. |
| ♞ | **[Tempo Chess](https://simple-games-dev.github.io/chess/)** | 2 | Chess with a clock. Premoves, move highlights, sudden-death finish. |

## How playing works

1. Pick a game.
2. **Play online:** create a room, choose how many players and an optional turn timer, then share the invite link. Friends join from any browser and pick a seat.
3. **Play on one device:** choose "Play on this device" and take turns.
4. Rooms disappear on their own about an hour after the last move, so there's nothing to clean up.

Every game has a "How to play" box on the page if you forget a rule.

## Under the hood

- Plain HTML, CSS and JavaScript — each game is a single file, no build step.
- 3D boards (Ascent, Hedgerow, Ghosts) use [Three.js](https://threejs.org/).
- Online rooms and chat run on Firebase Firestore.
- This repo is just the front door: `index.html` plus the artwork in `images/`.

## Adding a game to the page

Copy one `<a class="game">…</a>` block in `index.html`, change the link, name, text and tags, and drop a 1312×784 picture into `images/`. The filter chips (Strategy, Classic, Hidden info, 3D) use the `data-t` tags on each card.

## A note on names

Some of these games are inspired by well-known board games. They're fan-made, free, unofficial projects and aren't affiliated with or endorsed by the original publishers. If you're a rights holder and want something changed, please open an issue.
