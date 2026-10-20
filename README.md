# Idea Corkboard

A cork wall for all the ideas. Type an idea, tap a color, and it gets pinned to the board.

**Colors**

| Color | Kind | Meaning |
| --- | --- | --- |
| Green | Repeatable | something you could do again and again (a habit, a series, a recurring event) |
| Pink | One-and-done | a single project or action |
| Yellow | Fragment | half an idea, waiting for its other half |

**Using it**

- Type in the bar at the bottom, then tap a color. Enter posts with the outlined color. `Alt+1/2/3` posts as a specific color.
- Drag notes anywhere. Tap a note to tie a red string to another note, change its color, edit it, or delete it (with undo).
- `N` jumps back to the input. `Ctrl`/`Cmd` + scroll, or the `+`/`−` buttons, zoom the wall.
- The `⋯` menu exports and imports the board as JSON and can tidy notes into columns by color.

**AI**

- **Prioritize** ranks every note and explains each rank in one line.
- **Connect the dots** pins dashed red strings between related ideas, labels each one, and lists the patterns it sees in the Case file panel.

Opened as a Claude artifact, the AI runs on the viewer's own Claude account. Opened anywhere else (GitHub Pages, a local file), it asks once for an Anthropic API key, keeps it in that browser's local storage, and calls the Messages API directly from the page.

**Storage**

The board saves in the browser's local storage. Inside a Claude artifact it also saves to the viewer's private storage on their Claude account. Use Export JSON for backups.

It's a single `index.html` with no build step. Open it in a browser or serve the folder with any static host.
