# Project 4 — Pit Stop Analysis

Analysis of pit stop performance during the 2023 Qatar Grand Prix, focused on pit stop duration, team efficiency, and consistency. Builds on cleaned lap data from Project 1.

## What I did
- Matched each driver's pit-in lap to the following pit-out lap to calculate pit stop duration
- Handled edge cases: drivers starting from the pit lane (no prior pit-in) and retirements during a pit stop (no following pit-out)
- Flagged and excluded outliers to avoid skewing team averages, while keeping them separately
- Calculated mean and standard deviation of pit stop duration for use in Monte Carlo race strategy simulation

## Key Insights
- Average fastest pit stop of 27.864 seconds was by Ferrari
- RBR showed the widest spread in pit stop, ~5-sec gap between VER's stops and PER's stops
- Outliers were RUS(lap 1 due to repair work), GAS(lap 44 - just above the threshold) and HUL(lap 13 due to 10-sec penalty) with pit stop time above the threshold calculated

## Charts
- Average pit stop time by team
- Pit stop consistency by team (box plot)
- Fastest single pit stop by team
- Pit stop duration across the race

## Data output
- 'pit_stops_2023_Qatar.csv' — cleaned pit stop data
- 'outliers_pit_stops_2023_Qatar.csv' — flagged outlier stops
- 'pit_stats.json' — mean/std pit duration, used in Monte Carlo race strategy simulation

## Tools Used
Python, FastF1, pandas, matplotlib, seaborn
