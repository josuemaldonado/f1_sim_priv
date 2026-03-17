# F1 Simulator

A browser-based Formula 1 Championship management and simulation tool. Track a complete F1 season — manage your driver grid, record race and sprint weekend results, and follow championship standings for both drivers and constructors.

No installation or build process required. The entire application runs from a single HTML file.

---

## Features

### Driver & Team Management
- Add, edit, and remove drivers with name, car number, constructor, team color, and nationality
- Load the full 2025 F1 grid with a single click
- Configure season year and scoring rules per session

### Race Input
- **Standard Grand Prix weekends** — enter finishing order via drag-and-drop
- **Sprint weekends** — record both the sprint race and the grand prix separately
- Assign fastest lap bonus (top-10 finishers only)
- Points calculated automatically based on the selected scoring system

### Scoring Systems
| System | Points Distribution |
|--------|---------------------|
| Standard | 25-18-15-12-10-8-6-4-2-1 |
| Legacy | 10-8-6-5-4-3-2-1 |
| Custom | User-defined |
| Sprint | 8-7-6-5-4-3-2-1 (fixed, official F1 format) |

Fastest lap bonus (+1 point) can be toggled on or off.

### Driver Standings
- Full championship table with position, gap to leader, wins, podiums, and sprint wins
- Race history visualization — last 16 races displayed as color-coded dots (gold = win, green = podium, cyan = points finish, orange = sprint result)

### Constructor Standings
- Combined team points from both drivers
- Constructor wins, driver chips, and progress bars

### Race History
- Chronological log of all completed races (newest first)
- View full results for any race
- Edit race results, reset points, or delete races after submission

### Data Persistence
- Auto-saves to `localStorage` on every change with a timestamp indicator
- Export season data as a JSON file for backup
- Import a previously exported JSON to restore a season
- Full season reset option

---

## Usage

1. Open `f1-simulator.html` in any modern browser — no server needed
2. Go to **Setup** to add drivers or load the 2025 preset grid
3. Configure your scoring system and season settings
4. Go to **Race Input**, choose the weekend type (Standard or Sprint), and enter finishing order
5. Submit the race — standings update automatically
6. Track progress in **Driver Standings**, **Constructor Standings**, and **History**

---

## Tech Stack

- Vanilla HTML5, CSS3, and JavaScript — no frameworks or dependencies
- Google Fonts: Orbitron, Barlow, Barlow Condensed
- `localStorage` for persistence
- Deployed via Netlify

---

## Changelog

### March 17, 2026
- **Added sprint race support** — Race Input now includes a weekend type toggle between Standard GP and Sprint Weekend. Sprint weekends record both a sprint race result and a grand prix result. Sprint wins are tracked separately in driver standings. Sprint points follow the official F1 format (8-7-6-5-4-3-2-1).

### March 16, 2026
- **Netlify deployment** — Added `_redirects` configuration for URL routing on Netlify hosting.

### March 12, 2026
- **Initial release** — Full application including driver management, race input with drag-and-drop, driver standings, constructor standings, race history, multiple scoring systems, fastest lap bonus, export/import, and localStorage persistence.
