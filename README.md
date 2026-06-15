**[Home](https://yvesmango.github.io/) >> [Projects](https://yvesmango.github.io/projects) >>  Somerville Schools Traffic Safety**

# MBTA Park Accessibility

**Goal**: To evaluate walking access to parks from every MBTA station in Boston, Cambridge, and Somerville, and identify where the system excels — and where it falls short.

## Introduction

As Boston prepares to host the 2026 FIFA World Cup, millions of visitors will rely on the MBTA. This project measures how well the transit system connects riders to greenspace — from conservation land to soccer fields. Using open‑source tools, we generated 5‑, 10‑, and 15‑minute walking isochrones from 150+ stations and intersected them with state‑wide open space data. The result is a clear, data‑driven picture of transit‑based park access across the MBTA.

## Data Sources

- **MBTA Stations** : Rapid transit station locations (MBTA GIS data).
- **Open Space (Parks)** : MassGIS Protected and Recreational OpenSpace dataset (DCR).
- **Pedestrian Network** : OpenStreetMap footpaths and sidewalks accessed via OSMnx.

## Methodology

1. **Data Collection** : Downloaded MBTA stations, open space polygons, and pedestrian network data.
2. **Isochrone Generation** : Created 5‑, 10‑, and 15‑minute walking isochrones from each station using network‑buffered nodes and edges (inspired by Kuan Butts) instead of convex hulls — preserving gaps and avoiding overestimation of walkable area.
3. **Park Access Analysis** : Intersected isochrones with open space boundaries to determine which stations provide access within each time band.
4. **Visualization** : Produced static maps, a faceted dot plot, and a system‑wide summary table.

## Key Findings

- **98.6%** of MBTA stations (278 out of 282) reach a park within a 15‑minute walk.
- **90.5%** reach a park within **5 minutes**.
- Only **2 stations** have **no park access** within 15 minutes — these are true “transit‑park deserts.”
- The **Green Line E** and **Red Line** each contain one of these outlier stations.
- The MBTA overwhelmingly succeeds at park connectivity, with gaps isolated to specific stations rather than systemic failures.

## Outputs

- [Executive Summary](./executive-summary.md)
- [Interactive Map (coming soon)]() – planned Streamlit app
- [Analysis Notebook](./analysis.md)

## Technologies Used

`Python`, `GeoPandas`, `OSMnx`, `Matplotlib`, `Streamlit`, `REST APIs`, `Jupyter`

## License

MIT License