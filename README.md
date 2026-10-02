# Claude's Playpen

Four games and four toys that run in the browser. Each one is a single HTML file with no dependencies and no build step. Open `index.html` and pick one.

## Games

| Game | What it is |
| --- | --- |
| [Orbit Golf](orbit-golf.html) | Nine holes of mini golf in space (par 23). Drag back and let go to shoot, and bend the shot around planets' gravity. Suns burn you up, one hole has a wormhole, and on another the cup orbits a planet. |
| [Delve](delve.html) | A turn-based roguelike: 8 procedurally generated floors, 9 kinds of monster, weapons, armour, potions and unidentified scrolls. A dragon waits on the last floor. Death is permanent. |
| [Light Cycles](light-cycles.html) | Tron-style arena: you against 3 bots, or 2 players on one keyboard. The bots flood-fill the arena to pick moves and try to cut you off. First to 5 rounds wins. |
| [Hexsweeper](hexsweeper.html) | Minesweeper on a hexagonal board, in 3 sizes. Includes chording, long-press to flag, keyboard play and best times. |

## Toys

| Toy | What it is |
| --- | --- |
| [Sandbox](sandbox.html) | A falling-sand world with sand, water, oil, stone, plants, fire and lava. Water hitting lava turns to steam and leaves stone behind. Oil floats on water and burns. Plants spread by drinking water. |
| [Murmuration](murmuration.html) | Up to 2,400 starlings flocking at dusk (boids with a spatial hash). Your pointer is a hawk and the flock scatters around it. When you stop moving, a hawk on autopilot takes over. |
| [Life Sequencer](life-sequencer.html) | A 16-step, 12-pitch sequencer. At the end of each bar the grid takes one step of Conway's Game of Life, so the melody keeps rewriting itself. Audio is scheduled with Web Audio. |
| [The Lost Semicolon](semicolon.html) | A short text adventure. You're a semicolon that fell out of line 42 of `main.js`. There are 50 points to find and a rubber duck to talk to. |

## Running it

Open `index.html` in a browser. To serve it locally:

```sh
python3 -m http.server
```

To put it online, turn on **GitHub Pages** in the repo settings (Settings → Pages → deploy from the `main` branch, root folder).

## Controls

- **Orbit Golf:** drag anywhere to pull back the shot; the dotted line previews the first part of the flight. `R` restarts the hole.
- **Delve:** arrows, WASD, vi keys or the numpad to move (`y u b n` for diagonals); walk into monsters to attack. `q` drinks a potion, `r` reads a scroll, `z` rests, `>` goes down stairs. On touch, tap in the direction you want to move.
- **Light Cycles:** arrows or WASD to steer and `space` to boost. In 2-player, cyan uses WASD + `space` and magenta uses the arrows + `enter`. On touch, swipe to turn and tap to boost.
- **Hexsweeper:** click to dig. Right-click, long-press or turn on flag mode to flag. Click a number whose mines are all flagged to clear its other neighbours.
- **Sandbox:** drag to pour. Keys `1`–`8` pick an element, `space` pauses.
- **Murmuration:** move the pointer through the flock. The *field notes* panel has sliders for cohesion, alignment, separation, fear and flock size.
- **Life Sequencer:** click or drag on cells to draw, then press play (it needs sound). `space` toggles playback. Arrow keys and `enter` also edit the grid.
- **The Lost Semicolon:** type commands like `look`, `east`, `take duck`, `talk to duck`. Up and down arrows scroll through your command history. Some shell and git commands work too.
