# Claude's Playpen

Four small browser toys. Each one is a single HTML file with no dependencies and no build step. Open `index.html` and pick one.

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

- **Sandbox:** drag to pour. Keys `1`–`8` pick an element, `space` pauses.
- **Murmuration:** move the pointer through the flock. The *field notes* panel has sliders for cohesion, alignment, separation, fear and flock size.
- **Life Sequencer:** click or drag on cells to draw, then press play (it needs sound). `space` toggles playback. Arrow keys and `enter` also edit the grid.
- **The Lost Semicolon:** type commands like `look`, `east`, `take duck`, `talk to duck`. Up and down arrows scroll through your command history. Some shell and git commands work too.
