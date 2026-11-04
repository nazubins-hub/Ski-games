# Ski games

Small browser games and tools for teaching skiing, published with GitHub Pages.

| Game | What it teaches |
| --- | --- |
| [Edging](edge-rate/) | Edge control, and the rate of edging: tip and flatten the skis progressively, not abruptly. |
| [Rotary](rotary/) | Turn shape and speed: skis toward the fall line speed up, across it slow down. Hold a steady speed as the pitch changes. (Leg rotation separate from the upper body isn't modeled yet.) |
| [Fore/Aft Pressure](fore-aft/) | Fore/aft pressure: keep the center of mass over the feet. Move forward as the slope drops away over a crest, let the feet come forward into a dip, and be centered at takeoff, because the air can't fix it. |
| [Ski-to-Ski Pressure](ski-to-ski/) | Pressure from ski to ski: more weight on the outside ski the harder the turn. The game's own timing target is an early move onto the new outside ski at each transition. The rear view shows the long outside leg and short inside leg. |
| [Magnitude of Pressure](pressure/) | A sandbox with no score: edging and rotation, alone and combined, and the pressure they build against the snow. Carve, skid, pivot slip and edge set, with the skis bending and leaving tracks in a 3D view. |

## Layout

Each game is a folder with its own `index.html`, so its link is
`https://<user>.github.io/Ski-games/<folder>/`. The home page (`index.html`)
lists them all.

To add a game: create a folder, put the game in it as `index.html`, and add a
card for it to `index.html` and a row to the table above.

Game text follows the PSIA-AASI language and rules in `claude-context/`
(loaded through `CLAUDE.md`). Those files are copies; changes go to the
originals, not here.
