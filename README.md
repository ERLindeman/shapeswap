# Shape Swap

Shape Swap is a Capacitor/Vite canvas puzzle game built for mobile and web. Swap adjacent tiles of the same shape to make color groups, rack up points, and chase extinction bonuses—all while the app runs full-screen with Capacitor extras like the status bar hide.

## Gameplay
- Swap any two tiles that share the same shape.
- Create groups of 4+ matching colors to score.
- Identical-shape groups earn extra bonuses.
- Clear all tiles of a color to trigger a large extinction bonus.
- The pause menu opens on load and can be toggled by hardware/software back, any keyboard key, or the on-stage pause button; it includes Continue and Reset Game.
- Scores: `Game` is the current run, `Life` is lifetime and only increases.
- A Google AdSense unit is embedded at the top of the playfield without pushing the board down.

## Development
```bash
npm install
npm start        # runs Vite dev server
```

## Platform notes
- Built with Capacitor 7 and Vite. Android/iOS projects live in `android/` and `ios/`.
- Status bar is hidden on start via `@capacitor/status-bar`.
- Local storage persists lifetime score (`grid-life`) across runs; legacy `grid-best` is migrated on load.

## Controls
- Tap/click tiles to swap; pause via back button, keyboard key, or the pause icon beneath the board. Clicking outside the pause card dismisses it.

