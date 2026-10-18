# Orr's Place

A small furniture-placing game built on the floor plan of apartment 29 (floor 8, Ein Ganim 12, Petah Tikva).
Drag furniture onto the plan, move it around, rotate it, and see straight away if a piece hits a wall or sits outside the apartment.

When you're happy with the layout, press **Walk through in 3D** to walk around it in first person, or switch to a dollhouse view from above. People and dogs can be placed for scale.

Everything is in `index.html`, plus a local copy of the three.js 3D library in `vendor/`. There is nothing to install or build.

## Run it locally

Double-click `index.html`. It opens in your browser and works offline (only the fonts need internet; without it the page uses system fonts). Keep the `vendor` folder next to `index.html` so the 3D view works offline too.

## Run it on the web (GitHub Pages)

1. On GitHub, open the repository **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**, pick `main` and `/ (root)`, and save.
3. After a minute the game is live at `https://<your-username>.github.io/Orrs_place/`.

Any other static host works too: upload `index.html` and the `vendor` folder.

## How to play

| Action | How |
| --- | --- |
| Add furniture | Drag a card from the left panel onto the plan, or tap/click it to drop it in the middle of the view |
| Move | Drag a piece |
| Rotate | Drag the round handle above a selected piece, press `R` (90°) or `Q` / `E` (15°) |
| Resize, rename, recolor | Use the panel on the right |
| Nudge | Arrow keys (`Shift` for 25 cm steps) |
| Duplicate / remove | `Ctrl+D` / `Delete` |
| Undo / redo | `Ctrl+Z` / `Ctrl+Shift+Z` |
| Pan and zoom | Drag empty space, scroll wheel or pinch, `F` to fit |

- **Snap** keeps pieces on a 5 cm grid and pulls them flush against walls.
- A piece turns **red** when it overlaps a wall, a built-in fixture (kitchen counters, toilets, showers) or goes outside the apartment.
- Your layout saves automatically in the browser. Use **Save / Load** to copy or download it as JSON and load it on another device.
- **Height** in the right panel sets how tall a piece is in 3D (handy for people figures).
- **Example layout** fills the apartment with a furnished starting point; **Clear** empties it (both can be undone).

## The 3D walk-through

| Action | How |
| --- | --- |
| Look around | Click the view, then move the mouse (`Esc` frees the mouse). On phones, drag |
| Walk | `W` `A` `S` `D` or arrow keys, `Shift` to hurry. On phones, the stick at bottom left |
| Eye height | **Adult eyes** (162 cm), **Child** (105 cm) or **Dog** (42 cm) |
| Dollhouse | Look down at the whole flat with the ceiling off; drag to turn, scroll or pinch to zoom |
| Back to the planner | **Back to plan** or `Esc` |

You start just inside the front door. Only walls are solid: you can walk through doors, furniture and fixtures, so a half-open door never traps you outside a room. Figures in the **People & pets** group (175 cm adult, 120 cm child, a large and a small dog) appear in 3D with a bit of idle motion.

The plan has no height drawings, so the 3D view assumes 2.60 m ceilings, 2.10 m door tops and windows from 0.90 m to 2.10 m.

## About the plan

The walls, doors, windows and fixtures were traced from the architect's standard plan (scale in centimetres). Some parts of the drawing were cut off at the page edge, so the laundry room and the service balcony are approximate. The stairwell, lobby and elevator belong to the building and are shown hatched.
