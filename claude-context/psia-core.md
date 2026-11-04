<!-- Generated copy of Ski-Instruction/context/psia-core.md (2026-11-04). Don't edit here: edit the original on Nicholas's Mac and re-run scripts/sync-context.sh. -->

# PSIA core context for ski learning games

Shared by every game in Nicholas's ski-teaching work (Ski Playground, the web Ski Fundamentals Learning Games, and future ones). It sets the PSIA language a game may use and the PSIA rules a skier or skiing model must follow. Game-specific details live in each game's own context file.

Current for the 26-27 season (PSIA-AASI national documents, checked 2026-11-03).

**How to read this file**
- Text in double quotation marks is verbatim from a PSIA-AASI or PSIA-RM source. Game copy examples are in *italics*. Everything else is design guidance.
- Source keys: ATM6 = Alpine Technical Manual Ch. 6 Movement Analysis · LMA = The Language of Movement Analysis – Simplified · CS = Alpine Certification Standards v5 (10/02/25) · PG = Alpine Technical Skills Performance Guide (Jan 2024) · NAG = Alpine National Assessment Guide (26-27) · AAL = National Alpine Activities List v1.2a · Worksheet = Alpine MA Worksheet (Evan Vomacka, 2/6/2025).
- Full source texts and a cited framework are in `~/Documents/Ski-Instruction/` (`sources/text/`, `reference/framework.md`). Sessions that can't reach that folder (e.g. cloud sessions on a GitHub repo) must not add PSIA wording beyond this file; flag it for Nicholas to verify instead.
- PSIA documents describe what to **observe and say**, not physics equations. Game tuning numbers are game engineering, never PSIA facts.

---

## 1. Guardrails

1. **No invented PSIA claims.** If a source doesn't say it, the game doesn't say PSIA says it. Coaching ideas and physics are fine; label them as the game's own.
2. **Current terms only:** five fundamentals, Indicators of Integration, National Alpine Activities List names, Level 1/2/3. Retired: "IDP", "Common Threads", and three skills offered *instead of* the five fundamentals.
3. **Turn phases:** Initiation, Shaping, Finish, Transition. Never "Completion" or "Control phase".
4. **Cause and effect runs body → skis.** ATM6: "Typically, body movement or position is the cause of ski performance and ski performance is the effect." Player inputs are body movements; what the skis do is the effect. Feedback names both, in that relationship.
5. **Objective feedback.** PG: "Uses objective, specific, technically accurate, and non-judgmental language." Its example: "CM over base of support" as opposed to "good balance". No empty words (better, smoother, cleaner, nice) without the movement.
6. **Not a certification.** Games can borrow PSIA structure (activities, the six-point scale, level names) but never say a player is certified, passed, or assessed by PSIA, and never use PSIA-AASI logos.
7. **Shipping wording.** Standards and activity pages are PSIA-AASI documents. In shipped game text, prefer short terms and the game's own descriptions; check with Nicholas before shipping long verbatim passages.

## 2. The five fundamentals (verbatim)

From CS p.16 and the 2023 Learning Connection document. The UI short labels are game shorthand.

| Skill | UI short label | Fundamental |
|---|---|---|
| Pressure Control | Fore/aft | "Control the relationship of the center of mass to the base of support to direct pressure along the length of the skis." |
| Pressure Control | Ski to ski | "Control pressure from ski to ski and direct pressure toward the outside ski." |
| Edge Control | Edging | "Control edge angles through a combination of inclination and angulation." |
| Rotational Control | Rotation | "Control the skis' rotation with leg rotation, separate from the upper body." |
| Pressure Control | Pressure magnitude | "Regulate the magnitude of pressure created through ski/snow interaction." |

Three skills (Pressure, Edge, Rotational/Rotary Control) group the five fundamentals. ATM6 ties each skill to something visible on the skis: "Observe how skis act on snow to see how much they are turned (rotational control), tipped (edge control), and bowed (pressure control)."

## 3. Indicators of Integration

The observable signs that the fundamentals are blended (CS p.16, PG p.3), used for the Integrated activities (Wedge, Wedge Christie, Basic Parallel, Dynamic Parallel):

1. "Both skis maintain contact with the snow."
2. "The lower legs show similar forward angles."
3. "Both skis are guided to begin the turn."
4. "A countered relationship is visible through the transition between turns."
5. "The legs show independent flexion and extension as the body moves from one turn to the next."
6. "The torso remains stable while the legs move freely beneath it."

Expected quality by level (PG p.4): Level 1 "Functional", Level 2 "Coordinated", Level 3 "Refined and Optimized". At Level 3 the PG describes blending with "no discernible variation in quality of blending across all turn phases, turn to turn, and all three activities".

Measurable checks for a body model:

| Indicator | Variable to model | Check |
|---|---|---|
| 1 Both skis on snow | per-ski contact | no lifted ski during Integrated activities |
| 2 Similar lower-leg forward angles | per-leg shin angle (needs fore/aft) | left vs right difference under a tolerance |
| 3 Both skis guided to begin the turn | per-ski rotation start | both skis start turning within a short window |
| 4 Countered relationship through transition | torso yaw vs ski yaw | torso faces more downhill than the skis through transition |
| 5 Independent flexion and extension | per-leg length | inside and outside leg lengths differ as the body moves turn to turn |
| 6 Stable torso, legs move freely | torso angular velocity vs legs | torso rotates much less than the skis |

## 4. Language

### 4.1 Core vocabulary (LMA, verbatim)

**Ski performance words**

| Which Ski? | Part of Ski | Action (Which Skill?) | Action Describers |
|---|---|---|---|
| Inside · Outside · Uphill · Downhill · Left · Right · Both Skis · Weighted/Unweighted | Center · Tip · Tail · Middle/Waist · Underfoot · Toe piece · Heel piece · Top/Bottom | Twist/Turn · Tip/Edge · Flatten · Bend · Slide · Slip | toward · about · away from · up · down · in · out |

**Body performance words**

| Which Joint? | Which Action? | Resulting Body Parts | Action Describers |
|---|---|---|---|
| left · right · uphill · downhill · inside · outside · upper · lower · ankle · knee · hip · spine · shoulder · elbow · wrist · neck | open · close · flex · extend · turn · tip · rotate | Legs · Torso · CM · Pelvis · Chest · Head · Arms | up · down · around · in · out · toward · away · left · right |

**DIRT quantifiers (LMA)**
- Duration ("length of time movement exists"): Long · Short · Throughout
- Intensity ("how much, magnitude"): a lot · a little · low · high · heavy · light · more · less
- Rate ("degree of speed, pace"): quickly · slowly · abruptly · progressively · rapidly
- Timing ("sequential relation to another event"): during · before · after · simultaneously · sequentially · same time · Initiation · Shaping · Finish · Transition

ATM6 adds Direction: "Direction of movement can be observed relative to the slope, the turn, or the ski orientation."

Notes: Toe piece and Heel piece are their own parts (the bindings), not other names for Tip and Tail. "Twist/Turn" is a source word. Tipping and turning can share one sentence; AAL writes "The legs tip and turn the skis while the torso remains stable…".

**Other source terms:** carving · skidding · slipping · edge release · edge engagement · fore/aft balance · athletic stance (ATM6) · gliding wedge · christie · corresponding edges · opposing edges · brushed arcs · guided · steered · countered relationship · Center of Mass · Base of Support (AAL) · inclination · angulation (CS).

### 4.2 Layered tiers

Players start with plain words and unlock PSIA vocabulary as they progress. The LMA words are already plain, so Tier 0 is mostly those words without the framework names. Unlocking adds labels; it never changes what a word means.

| Tier | Player-facing language | Example message |
|---|---|---|
| 0 · First tracks | LMA ski and body words, plain DIRT words; no fundamental names. Gloss jargon: Center of Mass → *your body's balance point* | *Your skis slid sideways after the turn.* |
| 1 · Level 1 language | Five fundamentals (short labels), turn phases, DIRT categories named, cause → effect | *Shaping: both skis slip. The edges stay low while the legs turn the skis quickly.* |
| 2 · Level 2 language | Two or more fundamentals through all phases, DIRT on each, Indicators of Integration named | *Edging and rotation: the skis tip progressively through shaping, then flatten abruptly at the finish.* |
| 3 · Level 3 language | Multiple fundamentals blended, turn to turn, prescriptions that change DIRT | *Turn to turn, the edge change comes later on your left turns, so the outside ski bends less in initiation.* |

Level scopes come from the scored MA criteria (PG, assessment forms):
- Level 1: "Observe and describe the application of one or more Technical Fundamental in all turn phases." Prescribe "related to one Technical Fundamental".
- Level 2: "Observe and describe the application of two or more Technical Fundamentals in all turn phases."
- Level 3: "Observe and describe the application of multiple Technical Fundamentals in all turn phases and from turn to turn."

**Open conflict:** the Level 1 learning outcome says "within all phases of the turn" in CS and PG, but "in a specific phase of the turn" in the NAG and the L1 form. Ask Nicholas before writing Level 1 copy that depends on it.

Keep game difficulty separate from cert levels: name terrain by color (green / blue / black) or skier zone (CS: "Beginner/Novice-Zone", "Intermediate", "Advanced"), and call vocabulary tiers *Level 1/2/3 language*, never *Level 1 certified*.

### 4.3 Wording feedback

ATM6 template: "Paint a picture using the facts: the specific movement, where it occurs in the turn, the part of the body involved, and the resulting action of the skis."

Pattern: `[Phase]: [Which ski] [ski action] [DIRT]. [Body part] [body action] [DIRT].` (effect, then cause); for a prescription, `[Body action + DIRT] so the [ski] [ski action].`

- One point at a time. ATM6: "Giving too much information often inhibits learning as much as not giving enough information."
- Balance first. ATM6: "Generally, movements that negatively affect athletic stance and overall balance demand high priority."
- Describe what happened, not the player. No "bad", "sloppy", "great".
- Timely: right after the turn or run (ATM6: "The most effective feedback is prompt").

## 5. Skiing model rules (ski performance)

Effects a model should produce from its physics, not paint on (ATM6):
- Turn shape: "a turn in the shape of a C, J, or Z (the C being the generally favored goal and the J and Z indicating potential turn mechanics to address)."
- Speed control: "Watch the path of the skis throughout turns to observe whether speed is controlled by turn shape or through braking maneuvers, such as slipping or excessive skidding." AAL, repeatedly: "Consistent speed is created by turn shape."
- Edge change: "Look to see if the edge release at the finish of one turn flows smoothly into edge engagement of the next turn."
- Edge match: "Notice whether the edge angle in the snow is similar for both skis, and if both skis tip onto edge at the same time."
- Spray: "Snow spraying directly to the side reveals the skis are slipping sideways. Snow spraying more toward the rear is better because it shows the skis are traveling forward and skidding less through the arc of the turn."
- Tracks: "Note the track width, turn shape, location of skidding or carving, and degree of skidding." "The depth of the tracks left in the snow indicates the weight distribution between skis."
- Rate: "Edging movements occur at a faster rate in short-radius turns than in long-radius turns."

Cause → effect rules (ATM6). Use them in the physics and in feedback:

| Cause (body) | Effect (skis) |
|---|---|
| "when a skier moves too far toward the inside of a turn, weight increases on the inside ski, which can cause the skis to slip." | Inside ski gains load, grip drops, skid |
| "if a skier starts a turn while sitting back, his center of mass will most likely be behind his base of support in the finish phase as well." | A fore/aft error carries through the turn |
| "A narrow stance restricts the skier's ability to acquire a sufficient angle for the ski edge to hold." | Less edge hold on firm snow |
| "A skier who is not in balance will commonly sit back or lean toward the inside of the turn." | The two common imbalances; make both possible and visible |
| "A skier may edge skis at turn initiation or delay the timing and not edge the skis until the shaping or finish phase." | Edge timing changes turn shape |

Speed bands for the Integrated activities (AAL): Wedge Turns "Slow enough to not allow the skier to easily balance in a parallel turn"; Wedge Christie "Faster than wedge turns"; Basic Parallel "Faster than wedge christie turns and slow enough that the turns remain skidded rather than carved"; Dynamic Parallel "Faster than basic parallel turns, with enough speed and edge engagement to bend the skis and create a carved arc without becoming edge-locked."

## 6. Turn phases in a game

PSIA names the phases but gives no numeric boundaries. Each game needs one convention, labeled as the game's, used everywhere (HUD, feedback, debrief, tests) and kept in one function.

Suggested convention (game design, not PSIA): **Transition** = the edge change, from release of the old edges until the new edges engage. **Initiation** = from new-edge engagement until the skis point within a set angle of the fall line. **Shaping** = through the fall line band. **Finish** = from leaving that band until the next release.

Log per turn and phase: edge angle and its rate, skid angle, pressure and each ski's share, turn radius and shape, spray direction, time in phase. DIRT words come from these: Duration from time in phase, Intensity from the peak, Rate from the rate of change, Timing from where in the phase it started.

## 7. Body model targets

The sources refer to lower legs, knees, hips/pelvis, torso, arms/hands, the Center of Mass and each foot, so a skier body should have them. What an observer looks for (ATM6):
- "The forward slant of the lower leg should be parallel, or close to parallel, to the forward slant of the spine."
- "The skier's hips, shoulders, and hands should remain relatively level (perpendicular to gravity) as the CM moves to the inside of the turn."
- "Observe whether body movements begin with the upper or lower body. Look for a stable upper body and active leg movements."
- "Excessive arm movements can also disguise what is truly happening because they don't always reflect the movements of the rest of the body."
- "Through turn initiation, a skier may direct the CM down the hill, toward the apex of the turn, or along the length of the skis."

## 8. Rating and progression

Six-point scale (NAG, verbatim):
1. "Essential elements were not observed or not present."
2. "Essential elements are beginning to appear."
3. "Essential elements appear, but not with consistency."
4. "Essential elements appear regularly at a satisfactory level."
5. "Essential elements appear frequently, above the required level."
6. "Essential elements appear continuously, at a superior level."

A game can rate a check by how consistently it appeared across turns. PSIA's pass line is a section average of 4. Use the scale's words; don't call the result a PSIA assessment.

Debrief categories modeled on the Worksheet: Turn Shape (Round, Z, Comma, Apostrophe, Closed, Open) · Turn Size (Small, Medium, Large) · Ski Relationship (Wedge, Parallel, Diverging) · Edge Relationship (Opposing, Corresponding) · Spray · Performance (Carved, Skidded) · Leg Steering · body and joint angles, each "Consistent" or "Inconsistent Where?".

Progression for tutorials, from ATM6's exercise line: "Stationary" → "Simple" → "Complex" → "Whole". Teaching fundamental to design around (CS): "Promote play, experimentation, and exploration."

## 9. Checklist before adding PSIA text or mechanics

- [ ] Every PSIA term is in §4, or found in `~/Documents/Ski-Instruction/sources/text/` (or flagged for Nicholas if that folder isn't reachable).
- [ ] Quotes are verbatim; anything else is worded as the game's own.
- [ ] Each message names a phase, a visible action and a DIRT word, with body as cause and skis as effect.
- [ ] Turn phase comes from the game's one shared phase function.
- [ ] No retired terms, no "certified", no empty praise words.
- [ ] The physics produces the effect; the UI doesn't just assert it.
