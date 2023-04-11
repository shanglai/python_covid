
Hi.
This is a brief exercise on some data from a recent Covid-19 challenge at Kaggle.
The main goal is to accurately model and predict Confirmed cases and Fatalities in a global scale.
This is a serious challenge that could potentially benefit society at large, and while it has already ended, it was good to understand more of the virus' propagation and the SIR model, and hopefully make useful contributions to help fight this pandemic.

This is broken into several steps:
1: EDA: A small exercise into distribution and trends on a country level.
File: covid_forecast_eda_davidlopez.ipynb
Status: Finished

2. Clustering: Grouping several countries by a non-exhaustive list of variables I deemed interesting; among those are, per country:
- GDP
- Health Expenditure
- Population size and density
- Country size
- Location (Coordinates)
- Detected cases and casualties, per week
- Cases increment, per week
- To be implemented: 
  - Median of cases per N (3 to 5) closer countries, 
  - Median of cases for countries closer, within M (700) km, Haversine distance
NOTES: It was recommended to analyze China independently, but I chose to let it anyway and see how it clusters.
Method: Fuzzy C-means
File: covid_forecast_clustering_davidlopez.ipynb
Status: In progress

3. Prediction
Create a class for SIR prediction model and fit for several countries and several clusters. Check against Test DS. Maybe also use a polynomial / non-parametric fit.
Method: SIR & Poly or some GLM
File: NA
Status: To be started

4. Fit models with Genetic Algorithm
Use a GA to fit the growth and decay parameters for all elements in each cluster.
File: NA
Status: To be started

Sources:
GDP and population: https://www.worldometers.info/gdp/gdp-by-country/
Health expenditure by country: https://en.wikipedia.org/wiki/List_of_countries_by_total_health_expenditure_per_capita
Population, density and size: https://en.wikipedia.org/wiki/List_of_countries_and_dependencies_by_population_density
File: covid_forecast_clustering_davidlopez.ipynb






