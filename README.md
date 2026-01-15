NBA 2026 Free Agent Backup PG Analysis - Kush Havinal

This project aims to identify optimal backup point guard (PG) free agent targets for the 2026 NBA season, operating under a specified salary cap of $18 million. 
The analysis focuses on players proficient in pick-and-roll (PnR) offense and effective shooting off the dribble, while also considering age and contract value for long-term strategic fit.

Data Sources
Spotrac.com: Used to obtain a list of 2026 free agent guards and their projected salaries.
NBA API (nba_api): Utilized to retrieve detailed player statistics for the 2024-25 season, including:
SynergyPlayTypes: For pick-and-roll (PnR) ball handler statistics (Points Per Possession, Possession Percentage, Turnover Percentage, Field Goal Percentage).
PlayerDashPtShots: For pull-up shooting splits (3-point percentage, 2-point percentage, frequency) and self-creation rates (shots after high dribble counts).
LeagueDashPlayerStats: For basic player information such as age, games played, and minutes per game.

Methodology
Salary Filtering: Free agents were initially filtered to include only those with projected salaries at or below the $18 million cap.
Player ID Matching: Identified NBA player IDs for the filtered free agents using the nba_api to facilitate data retrieval. Fuzzy matching and manual corrections were applied for improved accuracy.
Statistical Data Collection: Fetched PnR and pull-up shooting statistics for eligible players from the nba_api for the 2024-25 season.
Data Merging and Cleaning: Combined salary data with NBA API statistics. Players without significant PnR usage were filtered out.
Scoring Engine Development: A weighted scoring model was developed to evaluate players across three main categories:
Pick-and-Roll Proficiency (40 points): Assessed based on Points Per Possession (PPP), Possession Percentage, Turnover Percentage, and Field Goal Percentage.
Off-the-Dribble Shooting (40 points): Evaluated using Pull-up 3P% and 2P%, Pull-up Shot Volume (FGA Frequency), and Self-Creation Rate.
Contract Value & Age (20 points): Scored based on projected salary affordability and age, prioritizing players in their prime years with flexible contracts.
Player Ranking: Players were ranked based on their total combined score, providing a quantitative assessment of their fit as a backup PG.

Key Findings
Initial analysis identified 88 affordable free agent guards under the $18M cap.
After filtering for PnR usage and matching NBA API data, a candidate pool of 55 players was established.
The scoring engine effectively distinguished players based on their statistical profiles and contract and age considerations.
The top-ranked candidates demonstrated a strong balance across all scoring categories: PnR efficiency, off-the-dribble scoring ability, and favorable age and salary profiles.
Collin Sexton	75	28	33	14	17,737,500	26	0.932	0.386
Nah'Shon Hyland stands out as the top candidate, combining strong PnR and pull-up shooting metrics with an excellent value proposition given his age and projected salary. Other high-ranking players like Collin Gillespie and Gary Trent Jr. also present compelling cases. The visualization further highlights the strengths and weaknesses of the top candidates across key decision-making metrics.
