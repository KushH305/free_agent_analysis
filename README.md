# NBA 2026 Free Agent Backup PG Analysis

**Author:** Kush Havinal

## Overview

This project evaluates 2026 NBA free agent point guards to identify optimal **backup PG targets** under an **$18M salary cap**. The analysis prioritizes players who excel in **pick-and-roll offense** and **off-the-dribble shot creation**, while accounting for **age** and **contract value** to ensure long-term roster fit.

## Data Sources

* **Spotrac** — 2026 free agent guard list and projected salaries
* **nba_api** — 2024–25 season player data:

  * *SynergyPlayTypes*: Pick-and-roll efficiency and usage
  * *PlayerDashPtShots*: Pull-up shooting efficiency and volume
  * *LeagueDashPlayerStats*: Age, games played, and minutes

## Methodology

1. **Salary Filtering**
   Filtered free agent guards with projected salaries ≤ $18M.

2. **Player Matching**
   Mapped free agents to NBA player IDs using fuzzy matching and manual corrections.

3. **Stat Collection & Cleaning**
   Retrieved PnR and pull-up shooting metrics; removed players with minimal PnR usage.

4. **Scoring Model**
   Built a weighted scoring engine (100-point scale):

   * **Pick-and-Roll Proficiency (40%)**
     PPP, usage, turnover rate, FG%
   * **Off-the-Dribble Shooting (40%)**
     Pull-up 3P%/2P%, shot volume, self-creation rate
   * **Contract Value & Age (20%)**
     Salary efficiency and prime-age preference

5. **Ranking**
   Players ranked by total score to quantify backup PG fit.

## Results

* **88** free agent guards identified under the salary cap
* **55** players remained after PnR usage and data validation filters
* Top candidates showed strong balance across PnR efficiency, shot creation, and value

**Key Insight:**
**Nah’Shon Hyland** emerged as the top target, combining strong PnR and pull-up shooting metrics with excellent age and contract value. Other notable candidates include **Collin Gillespie** and **Gary Trent Jr.**

## Takeaway

This framework provides a repeatable, data-driven approach to evaluating NBA role players by aligning on-court impact with salary and roster construction constraints—specifically tailored for backup point guard decision-making.
* Rewrite it for a **resume project description**
* Tighten language for **NBA/front-office style** documentation
