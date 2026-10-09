# Code-samples-Tamim-Adnan
This repository presents code summaries from my published research, showcasing my skills in programming, data cleaning, preprocessing, visualization, and machine learning modeling.

## Project-1: Two-step clustering Model 
This project includes extensive data engineering tasks. To find out the socioeconomic patterns including urbanity, spatial distribution, racial composition, age, gender, education, language spoken, employment, and disability, this study has integrated data from Highway Performance Monitoring Systems (HPMS), NASA MEERA-2, and American Community Survey (ACS). 

### Data collection, processing 
Collected and processed over **8.48 million roadway records (2017–2020)** from the Federal Highway Administration's Highway Performance Monitoring System (HPMS). Integrated pavement condition, structural, and traffic data with NASA MERRA-2 climate records and U.S. Census Bureau American Community Survey (ACS) socioeconomic data.

Developed a geospatial data integration workflow using five-digit county FIPS codes to align datasets across geographic locations and study years. Performed data cleaning, missing-value imputation using linear interpolation, and Pearson correlation analysis to examine relationships among variables.

The final dataset combined **pavement, traffic, climate, and socioeconomic features** to support spatiotemporal analysis, pavement performance modeling, and infrastructure equity research. 

### Two-step Clustering Model
Developed a **two-step clustering framework** combining K-Means and Hierarchical Agglomerative Clustering to efficiently analyze a large-scale dataset. Initially, K-Means was applied to generate 10 pre-clusters, followed by hierarchical clustering to identify the final cluster groups based on similarity. Evaluated clustering performance using the **Elbow Method, Silhouette Score, and Davies–Bouldin Index** to determine the optimal cluster structure while balancing clustering quality and computational efficiency. 


