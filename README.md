# The Impact of SEPTA Bus Service Cuts on Travel Time and Commuting Equity in Philadelphia

**Project Website (GitHub Pages):** https://julia88888888.github.io/finalsite/FinalDraft.html

## Overview
This project evaluates how SEPTA’s proposed bus service reductions may reshape transit accessibility and commuting equity across Philadelphia. Due to persistent routing “outside of service area” errors, the final analysis emphasizes accessibility and service-frequency change patterns rather than network travel-time comparisons.

## Data Sources
- **SEPTA GTFS** (pre- and post-cut schedules): routes, trips, stops, shapes, stop_times  
- **SEPTA service change / reschedule dataset** (official): headway changes (peak & midday)  
- **ACS (U.S. Census Bureau API)**: tract-level demographic and socioeconomic indicators  
- **OpenStreetMap (OSM)**: street network used for network/accessibility analysis

## Methods (Brief)
1. Compare GTFS service levels before vs. after cuts (trip counts, route frequencies).
2. Extract peak/midday headways from SEPTA reschedule notes using text parsing; compute headway differences.
3. Join headway changes with route geometries and visualize spatial patterns using interactive maps.
4. Retrieve ACS tract data and examine relationships between income, transit dependence, and service reductions.

## Repository Contents
- `FinalDraft.ipynb` — full analysis and figures/maps  
- `Dataset/` — input datasets used in the notebook (GTFS, reschedule files, etc.)

## Notes / Limitations
Travel-time routing comparisons were not completed reliably due to repeated routing service-area errors; results should be interpreted as accessibility- and service-pattern focused rather than definitive travel-time impacts.
