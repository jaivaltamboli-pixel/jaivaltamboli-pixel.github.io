# Football Tactics & Strategies

A modern, futuristic football tactics website focused on readability, SEO structure, and tactical learning flow.

## ✅ What's updated

- Futuristic homepage redesign with cleaner visual hierarchy.
- Improved SEO metadata (title, description, Open Graph, canonical, robots).
- Better content readability via spacing, responsive typography, and semantic HTML structure.
- New **Champions League Prediction Bracket** frontend page:
  - `predictions.html`
  - Built as a backend-ready UI output
  - Team list is currently sample/static
  - Bracket rounds and champion card are ready for data wiring

## Backend integration idea for bracket teams

When your backend is ready, replace static team blocks in `predictions.html` with API-fed data.

### Suggested response shape

```json
{
  "season": "2026/27",
  "teams": [
    { "id": "rm", "name": "Real Madrid", "pot": 1 },
    { "id": "mci", "name": "Manchester City", "pot": 1 }
  ]
}
```

### Example rendering approach

1. Fetch teams from backend endpoint, e.g. `/api/ucl/teams?season=2026-27`
2. Map each team to a `.team` card in the team pool.
3. Persist user picks in localStorage first, then sync to backend later.
4. Add validation to ensure each matchup has exactly one winner selected.

## Pages

- `index.html` — redesigned homepage
- `predictions.html` — new UCL bracket page
- Existing tactical pages remain available via navigation links

## Note

If you want the same futuristic typography/spacing system applied to every existing tactical page (`defense.html`, `possession.html`, `finesse.html`, etc.), I can ship a second pass that standardizes each page on a shared stylesheet.
