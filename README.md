# Orr's Place

A small furniture-placing game built on the floor plan of apartment 29 (floor 8, Ein Ganim 12, Petah Tikva).
Drag furniture onto the plan, move it around, rotate it, and see straight away if a piece hits a wall or sits outside the apartment.

Everything is in one file, `index.html`. There is nothing to install or build.

## Run it locally

Double-click `index.html`. It opens in your browser and works offline (only the fonts need internet; without it the page uses system fonts).

## Run it on the web (GitHub Pages)

1. On GitHub, open the repository **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**, pick `main` and `/ (root)`, and save.
3. After a minute the game is live at `https://<your-username>.github.io/Orrs_place/`.

Any other static host works too: upload `index.html` and you're done.

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
- **Example layout** fills the apartment with a furnished starting point; **Clear** empties it (both can be undone).

## About the plan

The walls, doors, windows and fixtures were traced from the architect's standard plan (scale in centimetres). Some parts of the drawing were cut off at the page edge, so the laundry room and the service balcony are approximate. The stairwell, lobby and elevator belong to the building and are shown hatched.
