# spatial-data-handling
GIS and Remote sensing analysis
### Project Summary

#### Objective
The objective of this project is to analyze the demographic and geographic characteristics of Bungoma County in Kenya using geospatial data. The analysis focuses on population distribution, including total population, gender-specific populations, and population density (Pop/sqkm).

#### Data Source
The project utilizes a shapefile (`Bungoma.shp`) that contains geospatial data for Bungoma County. The data includes attributes such as county, sub-county, population counts by gender, and geometries representing the boundaries.

#### Data Preparation
1. **Reading Data**: The shapefile is read using GeoPandas, and initial data exploration is performed.
2. **Data Cleaning**: Unnecessary columns (`dhis2_id`, `scpcode`, `ctypcode`, `provpcode`) are dropped.
3. **Coordinate Reference System (CRS)**:
   - The original CRS is WGS 84 (EPSG:4326).
   - The data is reprojected to UTM zone 37N (EPSG:32637) for area calculation in meters.

#### Analysis
1. **Area Calculation**: The area of each sub-county is calculated in square kilometers.
2. **Population Density**: Population density is computed as the total population divided by the area in each sub-county.

#### Results Visualization
Two sets of visualizations are created to illustrate the results:

1. **Four-Panel Plot**:
   - **Population per sqkm**: Shows the density of population across sub-counties.
   - **Total Population**: Displays the total population in each sub-county.
   - **Female Population**: Highlights the female population distribution.
   - **Male Population**: Highlights the male population distribution.

2. **Two-Panel Plot**:
   - **Total Population**: Reiterates the total population distribution across sub-counties.
   - **Population per sqkm**: Reiterates the population density across sub-counties.

#### Key Findings
1. **Sub-county Differences**: There are significant differences in both total population and population density across the sub-counties.
2. **Population Concentration**: Certain sub-counties like Kanduyi have higher population densities, indicating more concentrated populations.

### Conclusion
This project effectively demonstrates the use of geospatial analysis to understand population distribution within Bungoma County. The visualizations provide clear insights into demographic patterns, which can be useful for urban planning, resource allocation, and policy-making in the region.
