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

**Sharing your board on the website**

`⋯` → Share on my website… downloads `board.json`, a copy of your board with your name on it. Upload it to this repo (Add file → Upload files) to publish it. Visitors who open the app see that board first and can play with it, but their changes aren't saved and never touch yours. Start my own board gives them an empty board of their own in their browser. Without a `board.json`, the app opens with example notes.

**AI**

- **Prioritize** ranks every note and explains each rank in one line.
- **Connect the dots** pins dashed red strings between related ideas, labels each one, and lists the patterns it sees in the Case file panel.

Opened as a Claude artifact, the AI runs on the viewer's own Claude account. Opened anywhere else (GitHub Pages, a local file), it asks once for an Anthropic API key, keeps it in that browser's local storage, and calls the Messages API directly from the page.

**Storage**

The board saves in the browser's local storage. Inside a Claude artifact it also saves to the viewer's private storage on their Claude account. Use Export JSON for backups.

**Install it as an app**

Once the page is hosted (GitHub Pages works), open it and install it:

- **Chrome or Edge (Mac, Windows, Linux):** click the install icon at the right end of the address bar, or `⋯` menu → Install as app.
- **Safari (macOS Sonoma or later):** File → Add to Dock.

It opens in its own window with its own icon and works offline. The AI buttons still need internet.

It's a single `index.html` with no build step, plus `manifest.webmanifest`, `sw.js` (offline cache) and `icons/`.
