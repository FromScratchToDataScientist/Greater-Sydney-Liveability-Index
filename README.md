# Greater Sydney Liveability & Resource Analysis

This project evaluates how well-resourced Greater Sydney SA2 regions are by integrating multiple government datasets into a spatial database and computing a composite liveability score. The aim was to quantify infrastructure and service availability and identify inequality in resource distribution across Sydney.

## Key Features

- Integrated diverse datasets including:

  - SA2 spatial boundaries

  - Population & income

  - Businesses by industry

  - Public transport stops

  - School catchments

  - Points of Interest (POIs)

- Designed a normalised PostgreSQL/PostGIS database with:

  - Primary & foreign keys

  - B-tree and spatial (GiST) indexes for performance

  - Cleaned and standardised inconsistent datasets

- Performed spatial joins to map stops, schools, POIs, and businesses to SA2 regions

- Engineered resource metrics, including:

  - Businesses per 1000 people in key industries

  - Transport stops per region

  - School catchments per 1000 young people

  - POI density

- Applied z-score normalisation and a sigmoid scoring function to compute final liveability scores per SA2 region

- Conducted statistical and correlation analysis between resource scores and median income

- Produced interactive maps and visualisations showing spatial inequality in infrastructure distribution across Sydney SA4 regions

## Tools Used

- PostgreSQL + PostGIS for spatial database

- SQL for data cleaning, joins, and metric engineering

- Python / R for statistical analysis

- GIS visualisation tools for choropleth mapping

## Key Findings

- Business density and school catchments had the strongest impact on regional resource scores

- Inner West SA4 showed consistently higher liveability scores

- City & Inner South and Eastern Suburbs displayed high inequality, with few highly resourced outliers

- Median income showed only weak correlation with resource availability, indicating other drivers of infrastructure distribution

## Outcome

Delivered a complete end-to-end spatial analytics pipeline — from raw geospatial data ingestion to database design, metric engineering, scoring models, and visual insight into urban infrastructure inequality.
