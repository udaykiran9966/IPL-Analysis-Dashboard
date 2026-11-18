# IPL Analysis Dashboard (2008-2024)

Power BI dashboard analysing 17 seasons of the Indian Premier League.

## Dataset
IPL matches and ball-by-ball deliveries data from Kaggle (public dataset, not real company data).
- matches: 1,095 rows, 20 columns
- deliveries: 260,920 rows, 17 columns

## Tools
Power BI, Power Query, DAX

## Data cleaning (Power Query)
- Made team names consistent in both tables (for example Delhi Daredevils to Delhi Capitals, Kings XI Punjab to Punjab Kings, Royal Challengers Bangalore to Bengaluru).
- Created a Season Year column from the match date, because the season column had mixed formats (2007/08, 2009/10).
- Cleaned venue names (removed city names and merged renamed stadiums).
- Replaced "NA" values: missing city with UAE, missing winner with No Result.
- Fixed errors in target_runs and target_overs.
- Trimmed extra spaces and joined matches and deliveries using match id.

## Dashboard
- 3 KPI cards: Total Matches (1,095), Total Seasons (17), Total Teams (15)
- Matches per Season (line chart)
- Most Wins by Team (bar chart)
- Toss Decision (donut chart)
- Top 10 Run Scorers (bar chart)
- Season Year and Venue slicers

## Key findings
- Mumbai Indians have the most wins (144), followed by Chennai Super Kings (138).
- Toss winners chose to field first in 64.29% of matches.
- V Kohli is the top run scorer with 8,014 runs.
- Matches per season were higher in 2011-2013 and 2022-2024.

## Dashboard preview
![Dashboard](Screenshot%202026-11-18%20151242.png)
