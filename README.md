# GTA: San Andreas Vehicle Stats Analysis and Visualisation

Explore the inner mechanics of Grand Theft Auto: San Andreas vehicles using Python and data science tools. This project combines exploratory data analysis (EDA) with a nostalgic return to one of the most iconic open-world games of all time.

## About This Project

As a long-time fan of the GTA series, I revisited San Andreas after exams and became curious about how vehicles are designed and balanced in-game. I decided to extract the vehicle statistics and explore them using data science techniques - combining my passion for games with analytics.

This repository contains:
- A cleaned and well-structured dataset of 162 vehicles from GTA: San Andreas
- A full EDA notebook with insightful plots and comparisons
- Feature analysis and exploration of vehicle behavior and performance
- Fun and technical insights into Rockstar's vehicle logic

## Repository Contents

- **gta_sa_car_analysis_and_visualisation.ipynb** - Main analysis notebook: Full EDA including descriptive statistics, visualizations, relationship analysis, and ranking of cars by performance metrics (speed, weight, durability, etc.). This is the core of the project.
- **gtasa_cars.ipynb** - Data preparation notebook: Loads the raw CSV, performs cleaning (handling missing values, renaming columns, type conversion), and exports the cleaned dataset as gta_sa_vehicle_stats_ready.csv. Includes a quick test of the data.
- **gta_sa_vehicle_stats.csv** - Raw dataset extracted from gta.fandom.com using web scraping. This file contains unprocessed stats of 162 in-game vehicles.
- **gta_sa_vehicle_stats_ready.csv** - Cleaned dataset, ready for analysis. All values are processed, standardized and formatted for EDA.

## Dataset Overview

The dataset includes 35 columns of technical data per vehicle, such as:
- mass_(kg), acceleration(ms^2), max_velocity(km/h)
- drive_type, engine_type, brakes_deceleration
- collision_damage_multiplier, traction_multiplier, ABS, etc.

Each row represents a vehicle. These stats come from internal game config files and define physics behavior, handling, and damage systems in-game.

The data is suitable for:
- Exploratory Data Analysis
- Reverse engineering game mechanics
- Machine learning or clustering
- Game physics modeling

## Highlights

- Found some surprising trends - e.g., no strong link between acceleration and top speed.
- Identified outlier vehicles that are extremely fast, slow or durable.
- Grouped cars by drivetrain and performance.
- Used visualizations to explain how the game’s vehicle logic works.

## Data Source & Collection

- Source: https://gta.fandom.com/wiki/Vehicle_Stats_in_GTA_San_Andreas
- Collection Method: Data was scraped using pandas.read_html(), then cleaned and transformed for analysis (standardized column names, filled missing values, converted types).

## Final Note
This project was born out of my love for games and data. It’s been fun turning GTA: San Andreas into a playground for analytics - looking at cars not just for how they drive, but how they’re built under the hood.

