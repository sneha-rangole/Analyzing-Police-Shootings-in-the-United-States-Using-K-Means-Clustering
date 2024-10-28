# Project Description: K-Means Clustering Analysis of Police Shooting Data

## Overview
This project focuses on clustering data into disjoint sets, where data within a set is more similar to each other than to data in other sets. Clustering, a form of unsupervised learning discussed in Chapter 12 of the class reference text, allows me to uncover meaningful patterns in the data without predefined labels. I specifically implement k-means clustering, as outlined in Chapter 12.4 of the text and supported by various instructional videos.

## Data Sources
For this project, I analyze two datasets:
1. **Locations of Political Violence in India (2016-2024)**: A dataset detailing incidents of political violence.
2. **Locations of Police Shootings in the Continental United States**: A dataset detailing incidents of police shootings across the US.

## Key Methodologies
- **Distance Calculation**: Utilizing the Geopy library, I can calculate geodesic distances between latitude and longitude coordinates, essential for clustering analysis.

## Issues Addressed
The analysis of police shooting data reveals several critical insights:
1. **State Incidents**: I examined which states exhibit the highest number of police shooting incidents, comparing results across different cluster configurations (2, 3, 4, 5, and 6 clusters).
2. **Age and Death Count Relationship**: Investigating the relationship between age, manner of death, and the number of fatalities in the top five states for each of the six clusters.
3. **Top States Over Time**: Analyzing trends in police shootings in the top five states for each year from 2015 to 2022.
4. **Race and City Correlation**: Assessing correlations between the top five cities, racial demographics, and the number of police shootings.

## Findings
1. **Cluster Analysis**: 
   - In my k-means clustering analysis, Cluster 2 frequently emerged as the largest across various models, with Florida notably represented, indicating significant regional issues. In the six-cluster model, California stood out in Cluster 1.
  
2. **Top States for Incidents**: 
   - From 2015 to 2021, California consistently recorded the highest number of incidents, followed closely by Texas and Florida, indicating persistent challenges related to police violence.
  
3. **Yearly Trends**: 
   - California led the incidents each year, with Texas and Florida regularly appearing among the top three states, highlighting ongoing policing issues.
  
4. **Racial Disparities**: 
   - The analysis indicated that police shooting incidents disproportionately affect Black individuals, particularly in cities like Los Angeles, Phoenix, and Houston, raising serious concerns about systemic discrimination in law enforcement.

5. **Urban Concentration**: 
   - Most police shooting incidents were found concentrated in urban areas, suggesting unique challenges in policing in these densely populated regions.

## Appendix A: Method
1. **Data Collection**: 
   - The dataset was sourced from the specified class link, focusing on the 'fatal-police-shootings-data-continental-US.csv' file.

2. **Data Preparation**: 
   - A thorough examination of the dataset was conducted to ensure completeness and accuracy, documenting all steps for reproducibility.

3. **Variable Creation**: 
   - Key columns for correlation analysis included age, race, state, year, manner_of_death, and gender.

4. **Libraries Used**:
   - **Pandas**: For data manipulation and handling missing values.
   - **Folium**: For creating interactive maps and visualizing data points.
   - **Scikit-learn**: For applying the K-means clustering algorithm.
   - **Seaborn**: For generating a color palette for clusters.

5. **Analytic Method**:
   - Data preprocessing, legend addition for clarity in maps, descriptive statistics to understand incident distribution, application of the K-means algorithm for clustering, and visualization of clustered data to identify spatial patterns across the United States.
"""
