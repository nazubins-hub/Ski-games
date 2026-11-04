<!-- Generated copy of Ski-Instruction/context/web-learning-games.md (2026-11-04). Don't edit here: edit the original on Nicholas's Mac and re-run scripts/sync-context.sh. -->

# Ski Fundamentals Learning Games context

Small browser games that each teach one PSIA Alpine fundamental. Repo: `github.com/nazubins-hub/Ski-games` (public, published with GitHub Pages). Read `psia-core.md` first: it holds the PSIA language, guardrails and model rules. This file covers the repo, its house style, and each game's PSIA anchors. Double quotation marks mean PSIA source wording (as in `psia-core.md`); current game copy is in *italics*.

Players: guests and instructors, layered. Plain language first; PSIA vocabulary unlocks as the player goes further (`psia-core.md` §4.2).

## 1. Repo layout

From the README: each game is a folder with its own `index.html`; the home page `index.html` lists all games. To add a game: create the folder, add the game as `index.html`, add a card to the home page and a row to the README table. `.nojekyll` makes Pages serve files as they are.

| Folder | Game | Fundamental (UI label) |
|---|---|---|
| `edge-rate/` | Edging | Edging |
| `rotary/` | Rotary | Rotation |
| `fore-aft/` | Fore/Aft Pressure | Fore/aft |
| `ski-to-ski/` | Ski-to-Ski Pressure | Ski to ski |
| `pressure/` | Magnitude of Pressure | Pressure magnitude (with edging and rotation) |

Ski Playground's skier (Godot) is built on the Magnitude of Pressure model. Keep vocabulary and state words consistent across both.

## 2. House style

Observed in the deployed `rotary`, `fore-aft`, `ski-to-ski` and `pressure` files on 2026-11-04. Check the code before relying on a detail; `edge-rate` wasn't re-read.

- **One self-contained `index.html`**: vanilla JS in an IIFE, no JS libraries, no build step. Only external resource: Google Fonts (Barlow, Barlow Condensed).
- **Rendering**: canvas 2D (`pressure` uses its own perspective projection for 3D); `requestAnimationFrame` with `dt` clamped to 1/30 s; device pixel ratio capped at 2.
- **Theme**: colours in CSS custom properties, light by default, dark through `prefers-color-scheme` and `[data-theme="dark"]`; colours re-read when the scheme changes.
- **Controls**: one pointer-captured control (slider, pad or wheel) with `role="slider"` and live aria values; `pressure` has two pads (Edge, Rotate) for two thumbs. Arrow keys (Shift for faster). Esc or P pauses. Space/Enter presses the visible card's button. Auto-pause on `visibilitychange`.
- **Flow**: menu card (title, one-line tagline, how-to bullets, Start run) → run with HUD and meter words → short flash messages → Fell card (cause, then advice) or Run complete card (one lead sentence) → best score per trail.
- **Trails**: Green / Blue / Black chips; each trail sets speed, length and turn count.
- **Storage**: `localStorage` keys `<game>.trail` and `<game>.best.<trail>` (JSON), every access in try/catch so the game works with storage blocked.
- **Navigation**: *← All games* links to `../`.
- **Spelling**: current copy uses British *centred*. PSIA quotes use American spelling ("center of mass"); keep quotes as written and pick one spelling for game copy.

## 3. Each game's PSIA anchors and language to review

Quotes below are the source lines each game rests on. "Review" items are wording in the current game that doesn't match the current sources exactly; raise them with Nicholas before changing them.

### Edging (`edge-rate/`)
- Models: how quickly the edge angle builds or eases, progressive vs abrupt. Cites ATM Ch. 6.
- Anchors: ATM6 "Rate is the speed at which movement occurs." · "Edging movements occur at a faster rate in short-radius turns than in long-radius turns." · "Look to see if the edge release at the finish of one turn flows smoothly into edge engagement of the next turn." LMA rate words: quickly · slowly · abruptly · progressively · rapidly.
- Language: already uses LMA words (*abruptly*) and ATM6's edge release / edge engagement. Fine.

### Rotary (`rotary/`)
- Models: ski direction relative to the fall line sets speed; hold a steady speed as pitch changes. Tagline *Turn shape controls speed.*
- Anchors: ATM6 "Watch the path of the skis throughout turns to observe whether speed is controlled by turn shape or through braking maneuvers, such as slipping or excessive skidding." AAL "Consistent speed is created by turn shape." Fundamental: "Control the skis' rotation with leg rotation, separate from the upper body."
- Review: the game teaches turn shape and speed, not leg rotation separate from the upper body. *Rotary* is fine as a name (the RM Curriculum Guide says "Rotary Control"), but a menu line naming the fundamental would show what's not modelled yet. Opportunity: draw the legs turning under a stable torso.

### Fore/Aft Pressure (`fore-aft/`)
- Models: a hips slider moves the body over the feet; crests, dips and air; stance panel with ankle, knee, hip angles, a plumb line and a CM ring; *shin ∥ trunk*.
- Anchors: the fore/aft fundamental (CM relative to the base of support). ATM6 "The forward slant of the lower leg should be parallel, or close to parallel, to the forward slant of the spine." (matches *shin ∥ trunk*) · "A skier who is not in balance will commonly sit back or lean toward the inside of the turn." · sitting back at initiation carries into the finish (`psia-core.md` §5). AAL Straight run leaper: "The Center of Mass remains balanced over the feet so the skis leave and return to the snow as a unit".
- Review: *back seat* is slang (ATM6 says "sit back"). *Nose press* / *tail press* are freestyle terms, not in the sources; fine as game terms, don't present them as PSIA. The control is labeled hips, but the fundamental is about the Center of Mass over the base of support; keep feedback about the CM (the stance panel already shows it).

### Ski-to-Ski Pressure (`ski-to-ski/`)
- Models: a slider splits weight between skis; the outside ski's target share rises with turn demand; each transfer graded early / on time / late; the rear view shows a long outside leg and a short inside leg.
- Anchors: the fundamental "Control pressure from ski to ski and direct pressure toward the outside ski." (the tagline uses it). ATM6 "when a skier moves too far toward the inside of a turn, weight increases on the inside ski, which can cause the skis to slip." (matches *washes out*). AAL "The skier moves the Center of Mass over the new stance ski during each pressure transfer." Indicator of Integration 5: "The legs show independent flexion and extension as the body moves from one turn to the next."
- Review: *Move to the new outside ski early at each transition.* The *early* timing comes from the retired PSIA-RM IDP ("Transfer weight early, tip feet and lower legs, and direct pressure towards the new outside ski"). No current national document says early, and AAL's Whitepass even describes "the delayed pressure transfer to the new outside ski". Keep the mechanic if Nicholas wants it, but present the timing as the game's coaching target, not a PSIA rule.

### Magnitude of Pressure (`pressure/`)
- Models: a scoreless sandbox: Edge tips the skis, Rotate turns them; carve radius from sidecut and edge; grip, skid and pressure in body weights; outside ski up to 65% of the load; ski bend shown 6×; states flat glide, pivot slip, skid, carve, edge set.
- Anchors: the fundamental "Regulate the magnitude of pressure created through ski/snow interaction." ATM6 "bowed (pressure control)". LMA actions "Tip/Edge", "Twist/Turn". AAL activities Sideslip w/ Edge Set and Pivot Slips.
- Review: the subtitle *Control how much pressure the skis build against the snow.* is a paraphrase; fine as game copy, but don't label it as the fundamental's wording.

## 4. Coverage and gaps

Each fundamental has a game; Rotary covers turn shape more than leg rotation. Not covered yet: the Indicators of Integration (blending), turn phases, DIRT as a set, two-ski relationships (opposing vs corresponding edges, the wedge and christie), and movement analysis itself (observe → describe → cause and effect → prescribe).

Ideas for Nicholas to choose from (not planned):
- **MA eye**: watch a short replay and build a statement from cards (phase · which ski · ski action · body action · DIRT), checked against the replay's own data. Matches his sentence-build game; a pass-the-phone two-player mode with no typing would suit chairlift use.
- **Phase call**: tap when Initiation, Shaping, Finish and Transition start on a replay (using one shared phase convention, `psia-core.md` §6).
- **Integration checks** inside Magnitude of Pressure: score the Indicators of Integration that the model can measure.

## 5. Language in short web games

- Menu card: plain description (Tier 0), then the fundamental verbatim on one line, labeled *PSIA-AASI Alpine fundamental*.
- Flashes and meter words: Tier 0–1, two to five words, LMA words where they fit.
- Fell card: cause → effect in one sentence (body → skis), then advice as a prescription with a DIRT word.
- Run complete: one lead sentence; optional "more" panel with Tier 2–3 detail.
- No grades in words (*bad*, *great*); scores are percentages or the six-point scale wording.

## 6. Checklist for a new or changed game

- [ ] Folder + `index.html` + home page card + README row.
- [ ] House style (§2): single file, no libraries, light/dark, keyboard, touch, pause, storage in try/catch.
- [ ] Every PSIA term is in `psia-core.md` §4; anything new is flagged for Nicholas to verify against his source library.
- [ ] Feedback follows `psia-core.md` §4.3.
- [ ] Tested with storage blocked, keyboard only, touch, dark mode, narrow phone width.

## 7. Where the context lives

The originals are in Nicholas's `~/Documents/Ski-Instruction/context/`. The repo's `claude-context/` holds copies made by `scripts/sync-context.sh`. Don't edit the copies in the repo; propose changes and Nicholas updates the originals and re-syncs.
