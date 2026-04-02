# Tesla Global Market Analysis: PCA & Polynomial Extrapolation (2015-2025)

## About the Project
This Data Science project aims to analyze the evolution, technical efficiency, and expansion of Tesla in the global electric vehicle market during the 2015-2025 period. Using a dataset that includes production volume, deliveries, battery capacity, range, and CO2 savings, we applied dimensionality reduction techniques and predictive models to uncover hidden patterns in market behavior and the company's technological advancement.

## Methodology
The analysis was divided into the following methodological phases:
1. **Exploratory Data Analysis (EDA):** Data cleaning and exploration of delivery distributions by model (Model S, 3, X, Y, Cybertruck), market share by region, and price vs. range segmentation.
2. **Principal Component Analysis (PCA):** Dimensionality reduction of numerical variables to identify the principal components that best explain the technological and market variance of the vehicles.
3. **Component Density Analysis:** Evaluation of visual clusters using Kernel Density Estimation (KDE) to understand how different models group together in the new two-dimensional space.
4. **Polynomial Extrapolation:** Projection of future battery capacities and their impact on the actual range of the vehicles.

## Key Findings

* **Operational Intensity vs. Efficiency:** The PCA successfully reduced the dataset's complexity, revealing that the First Principal Component (PC1) acts as an "Operational Intensity" index (strongly grouping production, deliveries, and CO2 saved). Meanwhile, PC2 represents a "Volume-Efficiency" axis. This dimensionality reduction allowed us to visually and mathematically segregate Tesla's performance thresholds across different markets.
* **Probabilistic Operating Ranges:** By applying Kernel Density Estimation and polynomial fitting to the Principal Components (PC1), we constructed a probability density function. This allowed us to mathematically define frequent operational thresholds and prove that PC1 coherently summarizes the overall volume of deliveries across all regions and vehicle models.
* **Range/Battery Evolution:** Through polynomial extrapolation, we modeled future efficiency. We found that in a baseline scenario (100 kWh), a range of 575 km is achieved. By projecting a future scenario where energy capacity is doubled (200 kWh), the range increases to 1,141 km (+98.4%). This demonstrates high efficiency retention despite the theoretical weight penalty of additional batteries.


##  Technologies & Libraries
* **Language:** Python 3
* **Data Manipulation:** Pandas, NumPy
* **Data Visualization:** Matplotlib, Seaborn
* **Machine Learning & Mathematics:** Scikit-Learn (PCA, PolynomialFeatures)
* **Environment:** Jupyter Notebook / Google Colab

## Repository Structure
* `ProyectoTesla.ipynb`: Main notebook containing all the code, visualizations, and explanatory comments.
* `tesla_deliveries_dataset_2015_2025.csv`: Original dataset used for the analysis.
* `Propuesta_Tesla.pdf`: Formal technical report of the project formatted as an academic paper, including the theoretical mathematical foundation (Available in Spanish).

##  Project Context & Role
This project was developed collaboratively as part of the *Computational Mathematical Methods for Data Science* course at IIMAS - UNAM (National Autonomous University of Mexico). Within this team setting, I served as the Lead Contributor, driving the end-to-end implementation of the project. My specific responsibilities and core contributions included leading the Data Wrangling, Exploratory Data Analysis (EDA), PCA modeling, KDE Density Analysis, and Polynomial Extrapolation. 


##  How to run this project locally
1. Clone this repository: `git clone https://github.com/your-username/tesla-analysis-pca.git`
2. Install the required dependencies: `pip install pandas numpy matplotlib seaborn scikit-learn jupyter`
3. Launch Jupyter Notebook: `jupyter notebook`
4. Open the `ProyectoTesla.ipynb` file and run the cells sequentially.
