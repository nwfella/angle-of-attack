# Angle of Attack
## An Artillery Game That Teaches Geometry

---

## 1. Elevator Pitch

> *Most artillery games hide the math behind sliders. Angle of Attack forces you to **think** like a gunner — using triangles, angles, arcs, and estimation to hit targets you can't always see. Every shot is a geometry lesson you survive by learning.*

---

## 2. Core Philosophy

The game doesn't *tell* you geometry. It *forces* you to use it.

There are no UI sliders for "angle = 37.2°" and "power = 80%". Instead, the player interacts with geometric tools and must derive the solution themselves. The game provides the **workspace** — the player provides the **understanding**.

Early levels hold your hand with visible grids and protractors. Late-game levels strip everything away, leaving only your intuition and a blank canvas.

---

## 3. Visual Style & Theme

| Aspect | Design |
|--------|--------|
| **Aesthetic** | Dark chalkboard green background (#2d4a3e) with white chalk lines. Think "battlefield drawn on a classroom chalkboard." |
| **Terrain** | White chalk contour lines on the board. Mountains, buildings, walls drawn in chalk sketch style. |
| **Projectiles** | Glowing chalk comet trails — white/blue streak with tiny particles that fade. |
| **Explosions** | Chalk splash — radial burst of white dust that erases a bit of the board. |
| **UI** | Chalkboard frame border. Tools look like real classroom instruments (protractor, ruler, compass). |
| **Font** | Chalk-like (e.g., "Chalkboard" or "Caveat" for headings, "Courier Prime" for data). |
| **Title Font** | Hand-drawn rough chalk lettering for "Angle of Attack" |
| **Palette** | #2d4a3e (board), #f5f5dc (chalk), #87ceeb (player), #ff6b6b (enemy), #ffd700 (bonus/gold) |

---

## 4. Core Gameplay Loop

```
┌─────────────────────────────────────────────────────┐
│  1. SURVEY the battlefield  ← estimate distances,   │
│     spot targets, note terrain                       │
│  2. AIM using geometric tools  ← protractor, ruler, │
│     compass, angle tables                            │
│  3. FIRE the cannon  ← watch trajectory, see your   │
│     geometry play out in real time                   │
│  4. ADJUST based on feedback  ← "short by 20m",     │
│     "over by 15°", "ricochet angle was 63°"          │
│  5. LEARN the principle  ← each level teaches ONE   │
│     new geometric concept before combining them      │
└─────────────────────────────────────────────────────┘
```

Each level is a *puzzle* — there is always a geometrically correct solution. The player discovers it through measurement, reasoning, and adjustment.

---

## 5. Progression System — The Geometry Curriculum

The game is structured as a **cannon academy**. You start as a Recruit and graduate as a Master Gunner. Each rank unlocks a new geometric principle.

### 🎖 Act I: Foundations (Recruit → Corporal)

| Level | Concept | What the Player Does | Geometry Taught |
|-------|---------|---------------------|-----------------|
| 1 | **Flat Range** | Flat terrain, stationary target. Use a protractor overlay to match the correct launch angle. | Complementary angles: launch angle + 90° = normal. 45° gives max range. |
| 2 | **Range Finding** | Target with known height. Use similar triangles with a ruler tool to estimate distance. | Similar triangles / proportions. "If my thumb at arm's length covers a 2m target, the target is ~20x thumb-width away." |
| 3 | **The Perfect Arc** | Target at known distance. Find the two angles that hit it (low angle vs high angle). | Quadratic nature of projectile motion — every distance has two solutions (low and high trajectory, except max range). |
| 4 | **Elevation** | Target is on a hill above you. Must account for height difference. | Angle of elevation — right triangles with opposite/adjacent. |
| 5 | **Depression** | Target in a valley below. | Angle of depression — same concept from above. |

### 🎖 Act II: Trigonometry (Sergeant → Lieutenant)

| Level | Concept | What the Player Does | Geometry Taught |
|-------|---------|---------------------|-----------------|
| 6 | **The Observation Post** | You're behind a hill. Use a forward observer (spotter) to triangulate the target's position. | Triangulation — using two known points and angles to find a third. |
| 7 | **Counter-Battery** | Enemy fires first. Watch their shot, note its arc peak and impact point, then deduce their position. | Reverse trajectory analysis — given the parabola, find the origin. |
| 8 | **Wind Deflection** | Crosswind pushes the shell sideways. Must lead the target. | Vector addition — the shell's velocity + wind velocity as vector components. |
| 9 | **The Ricochet** | A wall blocks direct fire. Bank a shot off a cliff face to hit the target around a corner. | Angle of incidence = angle of reflection. Mirror geometry. |
| 10 | **Moving Target** | A wagon/truck moves laterally at constant speed. Must lead it. | Relative velocity, lead angle calculation, time-to-intercept. |

### 🎖 Act III: Advanced (Captain → Major)

| Level | Concept | What the Player Does | Geometry Taught |
|-------|---------|---------------------|-----------------|
| 11 | **Multiple Ricochets** | Bounce a shot off TWO surfaces (like billiards) to hit a hidden target. | Compound reflection. Angle chasing — sum of interior angles. |
| 12 | **The Mortar** | Very high arc to clear a mountain directly in front. Must use steep launch angle. | High-angle fire — the 60°-75° regime where range decreases as angle increases. |
| 13 | **Crest Clearance** | A hilltop between you and the target. Must fire high enough to clear it while still hitting the target. | Parabolic envelope — the family of curves from a fixed point. Finding the minimum-angle solution that clears an obstacle. |
| 14 | **Defilade** | Target is in a trench. Must land the shell INSIDE the trench, not just near it. | Precision arc — understanding that steep angles land more vertically (for trenches) and shallow angles skip (for bunker windows). |
| 15 | **Time on Target** | Two cannons must fire so both shells hit simultaneously from different distances. | Time-of-flight calculations. T = (2·v·sin θ) / g. Coordinating two trajectories. |

### 🎖 Act IV: Mastery (Colonel → Master Gunner)

| Level | Concept | What the Player Does | Geometry Taught |
|-------|---------|---------------------|-----------------|
| 16 | **The Hidden Battery** | Only sound cues (enemy firing) give away position. Use time delay of sound vs shell arrival. | Speed-of-sound ranging. Difference-of-arrival hyperbolas — a 2D form of GPS trilateration. |
| 17 | **Parallax Ranging** | Move between two positions, measure the target's angular shift, compute range. | Parallax — small baseline × large angle = distance. The same technique used to measure stars. |
| 18 | **The Zero-In** | Three shots total. First known-miss, use the miss vector (dx, dy at impact) to compute the correction. | Iterative refinement. The correction triangle. Each miss gives proportional feedback. Minimizing error. |
| 19 | **Napoleon's Trick** | Fire at the base of a wall — the angled impact collapses it onto enemies behind. | Force vector resolution. Component of impact normal to the wall. |
| 20 | **The Impossible Shot** | Final boss level. The target is behind a castle, you're in a ravine, wind is howling, you have ONE shot. Must use every principle learned. | Comprehensive synthesis — every geometric tool in the arsenal. |

---

## 6. The Geometry Toolbox

Players have access to tools they **unlock and upgrade** throughout the game.

### 🔧 Core Tools (available from Level 1)

| Tool | Function | How It Teaches |
|------|----------|----------------|
| **Angle Finder** | Snap to the cannon barrel and read the current angle in degrees. | Shows the angle but makes YOU change it (no slider). |
| **Chalk Ruler** | Draw a line between two points on the board. Read the distance. | Forces you to measure — no "range to target" readout. |
| **Grid Toggle** | Overlay a 10m × 10m grid on the battlefield. | Visual reference for distance estimation. |
| **Shot Clock** | Slow-motion playback of your last shot, with arc traced. | See the parabola after the fact — learn from your geometry. |

### 🔧 Intermediate Tools (unlock Level 5+)

| Tool | Function | How It Teaches |
|------|----------|----------------|
| **Protractor** | Place on any point, draw an arc between two lines, read the angle. | General angle measurement anywhere, not just at the cannon. |
| **Compass** | Draw a circle of known radius centered anywhere. | Visualizing blast radius, arc clearance, equidistant points. |
| **Triangle Tool** | Mark three points, read all angles and side lengths. | Full triangle solution — see angle-side relationships. |
| **Spotter** | A secondary viewpoint you can place anywhere to see the battlefield from another angle. | Perspective change — targets invisible from the gun line become visible. |

### 🔧 Advanced Tools (unlock Level 10+)

| Tool | Function | How It Teaches |
|------|----------|----------------|
| **Angle Bisector** | Draw the bisector of any angle. | Reflection geometry — find the angle for ricochet shots. |
| **Parallel Line** | Draw a line parallel to any other through a point. | Creating reference frames for vector decomposition. |
| **Tangent Finder** | Draw the tangent to your arc at any point. | Find the impact angle — important for bunker/ricochet shots. |
| **Reflection Tool** | Mirror a point or line across any other line. | Direct solution for ricochet shots (reflect the target across the wall). |

---

## 7. The Mathematics Engine

Every core mechanic is backed by real physics with a teacher-friendly twist.

### Projectile Motion

```
x(t) = x₀ + v·cos(θ)·t
y(t) = y₀ + v·sin(θ)·t - ½·g·t²
```

- g = 9.81 m/s² (real gravity)
- Wind adds a constant x-acceleration (simplified but real)
- No damage numbers — feedback is visual and geometric
- Trajectory is always drawn with a chalk arc after firing

### The Teaching Moment

When the player fires, the **chalk arc stays** on the board. They can then:
1. Measure the arc with their tools
2. Compare it to their intended arc
3. See exactly where their geometry was wrong

A **Score Card** after each successful hit shows:
- Your estimated angle vs. the true angle
- Your estimated range vs. true range
- Error breakdown (in degrees and meters)
- "What You Learned" — a plain-language explanation of the geometry concept used

### Feedback Types

| Miss Type | Visual Feedback | Text Feedback |
|-----------|----------------|---------------|
| Short | Chalk impact mark in front of target | "Short by 30m. Try a steeper angle or more powder." |
| Long | Chalk impact mark behind target | "Over by 22m. Lower your angle or reduce powder." |
| Left | Impact left of target | "18m left. Wind from the west. Adjust azimuth 4° right." |
| Right | Impact right of target | "15m right. Wind from the east. Adjust azimuth 3° left." |
| Ricochet miss | Splash mark on the wall showing impact angle | "Incidence: 47°. Reflection: 47°. Target was at 63°. Off by 16°." |
| Crest hit | Hilltop chalk marks the cleared height | "Cleared by 4m! You needed an angle > 52° to clear the ridge." |

---

## 8. Game Modes

### 📚 Campaign Mode (The Academy)

- 20 levels as described above
- Each level has a **Learning Objective** shown at start
- After each successful hit: **Geometry Lesson Card** explains the principle
- Bronze/Silver/Gold based on:
  - **Bronze**: Hit the target (any way)
  - **Silver**: Hit in ≤ 3 shots
  - **Gold**: Hit in 1 shot (perfect geometry)

### 🎯 Practice Range

- Free-form environment
- Place targets anywhere
- All tools unlocked
- Experiment with angles, distances, wind
- **Sandbox mode**: see real-time trajectory before firing (teaching mode)
- **Challenge mode**: hidden trajectory, must use tools

### ⚔️ Duel Mode (Local Multiplayer)

- Two players, split screen
- Take turns firing at each other
- Each has their own chalkboard workspace
- Same terrain, mirrored
- Winner is first to land a direct hit
- **Teaching variant**: each player can see the OTHER's chalk lines after firing — learn from their geometry!

### 🏆 Daily Geometry Challenge

- One randomly generated scenario every day
- Leaderboard with fewest shots to hit
- "Fix This Shot" variant: someone already fired and missed — you must adjust their geometry
- Highlights a specific geometric principle

---

## 9. UI Layout

```
┌────────────────────────────────────────────────────────────────┐
│  🧮 ANGLE OF ATTACK — Level 7: Counter-Battery               │
├────────────────────────────────────────────────────────────────┤
│                                                                │
│   ┌────────────────────────────────────────────────────────┐   │
│   │                                                        │   │
│   │              [Chalkboard Battlefield]                  │   │
│   │                                                        │   │
│   │    🏴         ⛰️          🚩                           │   │
│   │   Player     hill       Hidden Target                  │   │
│   │    🔫  →  [trajectory]                                  │   │
│   │                                                        │   │
│   │   [Grid overlay toggle]  [Zoom: □□□□□□□□□□]           │   │
│   └────────────────────────────────────────────────────────┘   │
│                                                                │
├─────── TOOLBAR ────────────────────────────────────────────────┤
│  📐 Angle   📏 Ruler   ○ Compass   △ Triangle   🔍 Spotter   │
├─────── CANNON CONTROLS ────────────────────────────────────────┤
│  Angle: ___°    Powder: ___%    Azimuth: ___°                  │
│  [Estimated Range: ____ m]   [Estimated Time: ____ s]          │
│                                                                │
│  [🔫 FIRE!]        [🧹 Clear Marks]        [📖 Hint]          │
├─────── LAST SHOT ──────────────────────────────────────────────┤
│  Aim: 38° @ 80% powder                                         │
│  Result: SHORT by 42m (impact at 358m, target at 400m)         │
│  Tip: Try 44° for the same powder, or keep 38° with 95% powder │
└────────────────────────────────────────────────────────────────┘
```

---

## 10. The Special Sauce — Teaching Without Telling

Here's what makes this game genuinely educational rather than just a shooter with a protractor:

### a) The "Ghost Geometry" Reveal
After a successful shot, the correct geometric construction is overlaid in **gold chalk** on top of the player's own chalk marks. They can see *exactly* where their construction deviated from the true solution. This is the core learning feedback loop.

### b) Layers of Scaffolding

| Difficulty | Tools Available | Hints Given | Visual Aids |
|------------|----------------|-------------|-------------|
| **Story (Easy)** | All tools unlocked | Direct hint button available | Grid always on, arc preview available |
| **Normal** | Tools available but not all unlocked | Subtle hints ("Try measuring from the crest") | Grid toggle only |
| **Hard** | No tools except ruler | No hints | No grid, no arc preview |
| **Nightmare** | No tools, random wind, one shot only | Nothing | Firing blind — must estimate everything |

### c) The Geometry Journal
A persistent in-game notebook that auto-records:
- Every shot's parameters and results
- The geometric principle used
- A sketch of the solution
- Your accuracy over time (did you improve?)

Players can also **hand-draw notes** (freeform chalk) on the journal pages.

### d) Cross-Curricular Connections
Each level card shows a real-world application:
- Level 6 (Triangulation): "Surveyors use this to map land. GPS uses this in 3D."
- Level 17 (Parallax): "Astronomers use this to measure distance to stars."
- Level 9 (Ricochet): "Pool players use this. So do laser mirror systems."
- Level 18 (Zero-In): "This is the same math behind gradient descent in machine learning."

---

## 11. Technical Specifications

| Aspect | Detail |
|--------|--------|
| **Platform** | HTML5/Canvas (web + standalone) |
| **Input** | Mouse + keyboard drag for tools. Number pad or text input for angle/power. |
| **Rendering** | 2D Canvas with chalk-texture shader (CSS filter + programmatic dithering) |
| **Resolution** | Responsive — 16:9 with min 1024×768 |
| **Physics** | Client-side deterministic (same result every time for same inputs) |
| **Audio** | Chalk squeak on drawing, deep cannon boom, whistle of shell, chalky splat on impact |
| **State** | LocalStorage for save/progress. No backend needed. |
| **Difficulty** | Per-level parameterized (enemies, wind, terrain height, tool restrictions) |

---

## 12. Level Architecture (Technical)

Each level is defined as JSON:

```json
{
  "id": 7,
  "name": "Counter-Battery",
  "concept": "reverse_trajectory",
  "concept_label": "Reverse Trajectory Analysis",
  "description": "The enemy fired first. Watch their shot, find their gun.",
  "terrain": {
    "player_x": 100,
    "player_y": 0,
    "enemy_x": 700,
    "enemy_y": -40,
    "features": [
      { "type": "hill", "start": 300, "peak": 450, "height": 60, "end": 550 }
    ]
  },
  "wind": { "speed": 2, "direction": "left" },
  "tools_allowed": ["angle_finder", "ruler", "protractor", "triangle"],
  "grid_default": true,
  "difficulty": "normal",
  "lesson_card": {
    "title": "Finding the Hidden Gun",
    "explanation": "By watching the enemy shell's arc, you can work backward to find its origin. The peak of the arc gives you the angle. The impact point gives you the distance. Two knowns → one unknown.",
    "real_world": "This is called 'sound ranging' and was used in WWI to locate enemy artillery."
  },
  "gold_condition": "1 shot",
  "silver_condition": "3 shots",
  "hint": "Mark the peak of the arc and the impact point. The launch point lies on the line through these."
}
```

---

## 13. Enemy Types

| Enemy | Behavior | Teaches |
|-------|----------|---------|
| **Static Cannon** | Sits still, fires every 3 turns | Basic geometry |
| **Mortar Team** | Fires high arcs, harder to hit (small target) | Steep-angle precision |
| **Moving Howitzer** | Moves 1 square per turn | Leading / relative velocity |
| **Bunker** | Armored top — only direct hit through the slit counts | Impact angle matters |
| **Artillery Battery** | Multiple guns firing at once | Multi-target prioritization |
| **The Spotter** | Doesn't fire — calls in airstrikes. MUST be hit first. | Triangulation (it hides) |

---

## 14. Scoring & Progression

| Metric | Effect |
|--------|--------|
| **Shots taken** | Lower = better rank (Bronze/Silver/Gold) |
| **Tool use** | Minimal tool use = bonus points (you did the math in your head) |
| **Speed** | Faster solution = higher score |
| **Ghost accuracy** | How close was your construction to the gold solution? (≤2° error = bonus) |
| **Consistency** | Consecutive 1-shot kills = streak multiplier |

**Unlocks:**
- Each rank unlocks new tools
- Gold on every level in an act unlocks a bonus level
- Perfect campaign (all Gold) = "Master Gunner" title + special chalk color

---

## 15. Accessibility

| Feature | Implementation |
|---------|----------------|
| **Colorblind mode** | All feedback uses position/shape markers, not just color. Targets have distinct shapes (◯△◇). |
| **Slow mode** | Shell travels at 0.5x speed. Trajectory auto-traces in real-time. |
| **Voice narration** | Geometry lessons and feedback narrated via speech synthesis. |
| **Magnifier** | Hold Shift to zoom in on any board area for precise tool placement. |
| **Keyboard-only** | All tools and firing accessible via keyboard shortcuts. |

---

## 16. Example Level Walkthrough

### Level 9: The Ricochet (Angle of Reflection)

**Setup:** Player is behind a stone wall. Enemy is around a corner, tucked behind a cliff. No direct line of fire. A flat cliff face at 45° to the wall acts as a mirror surface.

**What the player must figure out:**
1. Direct fire is impossible (wall blocks).
2. They must bounce the shot off the cliff face.
3. Angle of incidence = angle of reflection.
4. Method: draw the target's reflection across the cliff face line, aim at the reflection.

**Geometric solution:**
- Cliff face is a line L: y = 0.5x + 200
- Target is at T(650, 250)
- Reflect T across L to get T'(350, 550)
- Aim cannon at T' — the shell hits the cliff face at the correct angle and deflects to T

**Teaching support:**
- Hint 1: "What happens when light hits a mirror?"
- Hint 2: "If the target were on the other side of the cliff, where would it be?"
- Reveal: Gold chalk shows the reflection construction

**Scoring:**
- 1 shot = Gold (reflection method)
- 2-3 shots = Silver (trial and error)
- 4+ = Bronze (got there eventually)

---

## 17. Post-Launch Content Ideas

| Feature | Description |
|---------|-------------|
| **Level Editor** | Design your own geometry puzzles. Share via URL. |
| **Workshop** | Community-created levels. Rated by geometric concept. |
| **Spherical Geometry DLC** | Curved terrain (planet surface). Great-circle trajectories. |
| **Ballistics Table DLC** | Historical artillery tables from real wars. Fire using historical methods. |
| **Multi-Player Contest** | Simultaneous fire. Both players set up on the same battlefield. |
| **iOS/Android Port** | Touch-based tool interface. Tilt to aim (gyroscope). |

---

## 18. Visual Mockup Concepts (Text Description)

### The Title Screen
A chalkboard with "ANGLE OF ATTACK" written in bold white chalk, surrounded by geometric doodles — a protractor, a parabola arc labeled "θ = 38°", a triangle with annotated side lengths, and a small cannon doodle in the corner. A chalk eraser rests on the bottom rail.

### During Gameplay
The terrain is crosshatched contour lines (like a topo map). The player's cannon is a simple sketch — trapezoidal barrel on a triangular carriage. When firing, the shell leaves a glowing white-blue trail that slowly fades to dim chalk. Impact creates a white starburst that erases underlying chalk lines in a small radius.

### The Ghost Geometry Reveal
Gold dashed lines overlay the player's white chalk. If the player drew a triangle connecting themselves, the target, and a hilltop, the gold lines show the *correct* triangle with subtly different vertex positions. The difference is immediately visible.

---

## 19. Development Milestones (If Built)

| Phase | Deliverable | Timeline |
|-------|-------------|----------|
| **Prototype** | Level 1-5 playable, basic tools, one terrain type | Week 1-2 |
| **Core Loop** | All tools, physics engine, scoring, ghost reveal | Week 3-4 |
| **Campaign** | Levels 1-20 fully designed and balanced | Week 5-6 |
| **Duel Mode** | Local multiplayer, practice range, daily challenge | Week 7-8 |
| **Polish** | Audio, chalk aesthetic final pass, accessibility, journal | Week 9-10 |

---

*"Geometry is the art of correct reasoning from incorrectly drawn figures." — Henri Poincaré*

*"Angle of Attack" — because the best way to learn math is to survive it.*
