# NBA Standings Analysis & Dashboard

A two-part data science project analyzing a full NBA regular season across all 30 teams, 6 divisions, and 2 conferences: a Python/pandas analysis notebook, and an interactive web dashboard built from the same dataset.

**[Live dashboard →](https://eheayie.github.io/nba-standings-dashboard/)**
**[Analysis notebook →](./analysis.ipynb)**

## Part 1: Analysis (`analysis.ipynb`)

Exploratory data analysis in Python, covering:
- Data cleaning and feature engineering with **pandas**
- Descriptive statistics and groupby aggregation across conferences and divisions
- Hypothesis testing (independent t-test) comparing East vs. West win percentages with **scipy**
- Visualization with **matplotlib** and **seaborn**
- Unsupervised learning: **K-Means clustering** (scikit-learn) grouping teams into performance tiers based on win percentage

## Part 2: Dashboard (`index.html`)

An interactive, publicly hosted visualization of the same dataset:
- Sortable-style standings tables for both conferences, with playoff / play-in / eliminated status
- All 30 teams ranked by win percentage in an interactive horizontal bar chart
- Division strength comparison
- Auto-generated insights: tightest playoff races, strongest and weakest divisions

Built with vanilla JavaScript, [Chart.js](https://www.chartjs.org/), and HTML/CSS — no build step, fully static.

## Data

Team-level season standings (wins, losses, win percentage, conference, division, playoff status) for all 30 NBA teams.

## Running locally

**Dashboard:** single static HTML file, no dependencies. Open `index.html` directly, or serve it:
```bash
python3 -m http.server 8000
```
Then visit `http://localhost:8000`.

**Notebook:** requires `pandas`, `matplotlib`, `seaborn`, `scipy`, and `scikit-learn`.
```bash
pip install pandas matplotlib seaborn scipy scikit-learn jupyter
jupyter notebook analysis.ipynb
```
