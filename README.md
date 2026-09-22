# NBA Standings Dashboard

An interactive data analytics dashboard visualizing a full NBA regular season across all 30 teams, 6 divisions, and 2 conferences.

**[Live demo →](https://eheayie.github.io/nba-standings-dashboard/)**

## What it does

- Displays sortable-style standings tables for both conferences, with playoff / play-in / eliminated status
- Ranks all 30 teams by win percentage in an interactive horizontal bar chart
- Compares average win percentage across all 6 divisions
- Auto-generates insights: tightest playoff races, strongest and weakest divisions

## Built with

- Vanilla JavaScript (data processing, DOM rendering)
- [Chart.js](https://www.chartjs.org/) for the win-percentage chart
- HTML/CSS (no build step — fully static, single-file site)

## Data

Team-level season standings (wins, losses, win percentage, conference, division, playoff status) for all 30 NBA teams.

## Running locally

This is a single static HTML file with no dependencies to install. Just open `index.html` in a browser, or serve it with any static file server:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.
