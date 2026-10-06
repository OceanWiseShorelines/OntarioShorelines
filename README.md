# Ontario Shoreline Cleanup Data Explorer

Interactive Shoreline Cleanup Data Explorer for Ontario.

## Coverage

- Toronto Neighbourhoods
- Ontario Lower and Single-Tier Municipalities
- 2018–2025

## Explorer features

- Geography switching
- Area search and highlighting
- Cleanup and litter metrics
- Mean and total measures
- Single-year and grouped-year analysis
- Dynamic choropleth mapping, legends, and popups

## Deployment

This repository is designed for GitHub Pages. `index.html` is self-contained and includes the web map data, styling, and application logic.

To publish with GitHub Pages, upload the repository contents to the repository root and configure Pages to deploy from the main branch/root directory.

## Updating the data

The source annual GIS summaries are produced in QGIS using Join attributes by location (summary). Each annual layer should be generated independently from the clean base geography and the cleanup points filtered to that year.


## October 2026 UI fix
- Grouped Years now uses one continuous dual-handle year track.
- Year ticks are displayed from 2018 through 2025.
- The legend refreshes from the selected Metric and Measure.
- Ontario subtitle updated for Toronto neighbourhoods and ON municipalities.


## Display notes
Ontario municipality names are formatted in title case in the interface. The legend heading displays only the selected metric; the selected measure still controls the values and class breaks.


Capitalization fix: Ontario municipality names are normalized at the geometry source before search options and popups are generated.


## Municipality capitalization
Ontario municipality names are formatted at display time with a regex-free title-case function. This applies to both the search autocomplete and map popups.
