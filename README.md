# Code-samples-Tamim-Adnan
This repository presents code summaries from my published research, showcasing my skills in programming, data cleaning, preprocessing, visualization, and machine learning modeling.

## Project-1: Two-step clustering Model 
This project includes extensive data engineering tasks. To find out the socioeconomic patterns including urbanity, spatial distribution, racial composition, age, gender, education, language spoken, employment, and disability, this study has integrated data from Highway Performance Monitoring Systems (HPMS), NASA MEERA-2, and American Community Survey (ACS). There are two publications on this project. 

Conference Paper: Uncovering Socioeconomic Features in Pavement Conditions Through Data Mining: A Two-Step Clustering Model
Doi: 10.1109/WSC63780.2024.10838835

Journal Paper: Paving Equity: Unveiling Socioeconomic Patterns in Pavement Conditions Using Data Mining 
Doi: https://doi.org/10.1061/JMENEA.MEENG-6708 

### Data collection, processing 
Collected and processed over **8.48 million roadway records (2017–2020)** from the Federal Highway Administration's Highway Performance Monitoring System (HPMS). Integrated pavement condition, structural, and traffic data with NASA MERRA-2 climate records and U.S. Census Bureau American Community Survey (ACS) socioeconomic data.

Developed a geospatial data integration workflow using five-digit county FIPS codes to align datasets across geographic locations and study years. Performed data cleaning, missing-value imputation using linear interpolation, and Pearson correlation analysis to examine relationships among variables.

The final dataset combined **pavement, traffic, climate, and socioeconomic features** to support spatiotemporal analysis, pavement performance modeling, and infrastructure equity research. 

### Two-step Clustering Model
Developed a **two-step clustering framework** combining K-Means and Hierarchical Agglomerative Clustering to efficiently analyze a large-scale dataset. Initially, K-Means was applied to generate 10 pre-clusters, followed by hierarchical clustering to identify the final cluster groups based on similarity. Evaluated clustering performance using the **Elbow Method, Silhouette Score, and Davies–Bouldin Index** to determine the optimal cluster structure while balancing clustering quality and computational efficiency. 

<img width="1654" height="951" alt="Two-Step Clustering Workflow" src="https://github.com/user-attachments/assets/54846e96-c833-46ff-9d8a-9f0605e30db1" />

## Project-2: Explainable AI Framework for Pavement Condition Analysis 

This project is also based on HPMS datasets including 2 and 3 year horizon IRI prediction. This study included data preprocessing such as removing missing values, categorical encoding, model development and optimization. 

There are two publications on this project.
Conference Proceedings: https://doi.org/10.1061/9780784486962.030 

Journal Version: 10.1016/j.rineng.2025.108666  

### Data Processing 
Prepared pavement datasets for **2-year (2017–2019) and 3-year (2017–2020) prediction horizons**. Since missing values were minimal, incomplete records were removed. Applied **Min-Max normalization** to scale numerical features between 0 and 1 while preserving their relative distributions. Although Min-Max scaling standardizes feature ranges, it remains sensitive to outliers. 

### Model Development 
#### Machine Learning Model Development

Developed and evaluated four machine learning models for pavement condition prediction across 2-year and 3-year prediction horizons:

- **Artificial Neural Network (ANN):** Implemented a multilayer neural network with input, hidden, and output layers to capture complex nonlinear relationships among pavement, traffic, structural, and environmental features.
- **Random Forest (RF):** Applied an ensemble learning approach using multiple decision trees and bootstrap aggregation (bagging) to improve prediction stability, reduce overfitting, and enhance generalization.
- **Extreme Gradient Boosting (XGBoost):** Implemented a gradient boosting framework that sequentially builds decision trees to minimize prediction errors, incorporating learning rate optimization and regularization.
- **Categorical Boosting (CatBoost):** Applied a gradient boosting algorithm using symmetric decision trees and ordered boosting to improve predictive accuracy and efficiently handle categorical features.

#### Model Performance Evaluation

Evaluated model performance using four statistical metrics:

- **R² (Coefficient of Determination):** Measures the proportion of variance explained by the model.
- **MAE (Mean Absolute Error):** Quantifies the average absolute difference between actual and predicted values.
- **MAPE (Mean Absolute Percentage Error):** Measures prediction errors as percentages of actual values.
- **WMAPE (Weighted Mean Absolute Percentage Error):** Measures total absolute prediction error relative to the total observed values.

These metrics were used to compare model accuracy and predictive performance across different algorithms and prediction horizons.
