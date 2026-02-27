# MLB Fastball Velocity & Movement Analysis — 2024 Season
**Tools:** Python, pandas, pandasql, matplotlib  
**Data:** Baseball Savant Leaderboards via Kaggle

## Question
Does fastball velocity correlate with movement deviation from league average?

## Data Source
Baseball Savant pitch movement leaderboard filtered to 2024 season, 
minimum 100 pitches thrown (428 qualified pitchers).

## Methodology
Pitchers were segmented into four velocity tiers using a SQL CASE statement:
- Elite Velocity: 95+ mph
- Above Average: 92–94 mph
- Average: 89–91 mph
- Below Average: under 89 mph

Movement was measured as deviation from league average in inches, 
both vertically (rise) and horizontally (tail).

## Key Findings
- **Elite velocity pitchers generate above average vertical movement** (+0.06 inches) 
  while below average velocity pitchers fall significantly short (-2.48 inches)
- **Harder throwers do not automatically dominate movement leaderboards** — 
  the top 10 vertical movement leaders averaged only 93.5 mph, suggesting 
  some pitchers compensate for average velocity with exceptional movement
- **Paul Skenes** (98.8 mph) showed the most extreme movement profile among 
  elite velocity pitchers with -4.6 vertical and +6.0 horizontal deviation
- **Horizontal movement shows no clear velocity trend** — suggesting 
  tail/cut is more mechanics-dependent than velocity-dependent

## Conclusion
Velocity and movement are related but not interchangeable. Elite fastballs 
tend to generate above average rise, but the best movement pitchers in MLB 
are often mid-90s arms with exceptional spin profiles rather than pure 
fireballers.
