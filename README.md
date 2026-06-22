# Rebuildle

An FRC-themed attribute-guessing game based on the 2026 *FIRST* Robotics Competition
game **REBUILT presented by Haas** — styled after The Blue Alliance.

Guess the hidden team by typing team numbers. Each guess reveals how that team's robot
compares to the mystery team across number, rookie year, and game attributes.

## Play
It's a single self-contained file — just open **`index.html`** in any modern browser.
No build step, no server.

### Modes
- **Daily** — one shared puzzle per day (same team for everyone), drawn from the
  recognizable-teams pool with a year-seeded rotation.
- **Free Play** — endless rounds; **Normal** (recognizable teams) or **Hard** (every team).
- 8-guess limit. Results share as an emoji grid.

### Comparison columns
Team · Rookie Year · Clearance · Serialization · Shooter · Team Color · Climb · Intake

- **Shooter** — `Turret` / `Double Turret` / `Dumper`. Single vs double turret is an
  orange *partial* match.
- **Team Color** — a set of 1–2 colors; green = same set, yellow = shares one, gray = none.

## Data
Robot attributes live in [`rebuildle_data.json`](rebuildle_data.json), exported by the
Rebuildle Data Logger and embedded into `index.html` as `RAW_DATA`. Team names, rookie
years, and robot photos are pulled live from the [The Blue Alliance](https://www.thebluealliance.com) API.

## Notes
*FIRST*, FRC, and REBUILT are trademarks of *FIRST*. This is an unofficial fan project.
