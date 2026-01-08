# Tennessee Voting Patterns Before and After Redistricting

## Motivation
Congressional redistricting reshapes how voters are grouped and represented, yet its effects are often discussed at a high level without examining how these structural changes relate to local election outcomes. I wanted to explore whether changes in congressional district boundaries are associated with observable differences in voting patterns at the county level.

By focusing on county-level data and statewide elections, this project aims to better understand how redistricting may coincide with changes in election margins and voter turnout.

## Questions
This analysis explores the following questions:

- Which Tennessee counties experienced changes in congressional district boundaries after redistricting?
- How did the number of congressional districts intersecting each county change between the 2018 and 2022 elections?
- Do counties affected by redistricting show different changes in election margins than counties that were not affected?
- Are changes in voter turnout different in counties that experienced boundary changes?

## Data
- **Tennessee Secretary of State**
  - County-level election results for the 2018 and 2022 Tennessee Governor elections
- **U.S. Census Bureau**
  - Congressional district boundary shapefiles
  - County-to-congressional-district crosswalk files

The governor elections were selected because they are statewide contests and include all counties.

## Data Cleaning and Preparation
- Standardized county identifiers across election and geographic datasets
- Filtered election results to include only relevant statewide races
- Aggregated vote totals at the county level
- Calculated:
  - Margin of victory
  - Total turnout
  - Percent change in turnout
- Created a county-level measure of redistricting exposure based on changes in the number of congressional districts intersecting each county

## Problems and Hurdles
- County identifiers were formatted differently across datasets and required standardization before merging
- Counties that intersect multiple congressional districts required careful handling to accurately measure fragmentation
- Geospatial files were large and required preprocessing to enable efficient analysis
- Turnout and margin changes may reflect factors beyond redistricting that are not captured in this dataset

## Technologies Used
- Python- Jupyter Notebook
- Pandas
- GeoPandas
- Matplotlib
- MS Powerpoint

## Conclusion
This analysis shows that congressional redistricting altered how some Tennessee counties were divided across districts and that counties affected by these changes often exhibited greater variability in election margins between 2018 and 2022. Changes in voter turnout were less consistently associated with redistricting exposure.

## Presentation
[View Presentation Slides](https://1drv.ms/p/c/4c46f7862bc1ce0b/IQD-uvYyHxtUQbqqioewauGoAcpXPLS_lKjoY4kR3kFr_nA?e=b6v1xE)
