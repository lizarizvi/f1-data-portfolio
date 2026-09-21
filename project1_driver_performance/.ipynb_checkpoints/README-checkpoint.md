# Project 1 — Driver Performance Analysis

Analyzed lap times, sector times, and consistency across all drivers in the 2023 Qatar Grand Prix using real F1 timing data (via FastF1 API).

## What I did
- Cleaned raw lap data (removed safety car laps, in/out laps)
- Compared drivers on pace, consistency, and sector-by-sector performance
- Identified where on track each driver gains or loses time

## Key insight
- PIA had the fastest average race pace while OCO was the most consistent among the top 10 finishers.
- RUS and LEC were the drivers among top 5 that showed the sharp upward trend which could likely be the tyre degradation.
- Among the top 10 finishers, BOT lost ~0.753 secs in sector 1 which was the biggest gap to PIA who was fastest.
- VER had the fastest lap overall with laptime of 84.319 seconds.

## Charts
See the 'charts/' folder for lap time distribution, driver consistency, lap time evolution, sector time heatmap, fastest lap comparison and pace vs consistency scatter plot.

## Data output
Cleaned dataset is saved to '../shared/cleaned_laps_2023_Qatar.csv' — used as input for Pit Stop Analysis and Lap Time Prediction.

## Tools used
Python, FastF1, pandas, seaborn, matplotlib