# SpaceX Falcon 9 First Stage Landing Prediction

## Project Overview
This repository contains my capstone project for the **IBM Data Science Professional Certificate**. The objective of this project is to predict whether the first stage of the SpaceX Falcon 9 rocket will land successfully. Since rocket launches cost upwards of $62 million and reusing the first stage saves a massive percentage of that cost, predicting landing success allows us to determine the cost of a launch.

## Project Pipeline & Architecture
The project is divided sequentially into the following Jupyter Notebooks and applications:

1. **01_data_collection_api.ipynb**: Fetching historical launch records via the SpaceX REST API and structuring the raw JSON responses.
2. **02_webscraping.ipynb**: Using BeautifulSoup to scrape Falcon 9 launch records from Wikipedia to supplement the dataset.
3. **03_Data wrangling.ipynb**: Data cleaning, handling missing values, creating binary landing labels, and preparing features.
4. **04-eda-with-sql.ipynb**: Uploading data to an SQLite database and running SQL queries to uncover insights into launch sites and payload metrics.
5. **05_edadataviz.ipynb**: Comprehensive Exploratory Data Analysis using Seaborn and Matplotlib to visualize data correlations.
6. **06_launch_site_location.ipynb**: Geolocation analysis mapping launch pad locations and safety distance buffers using Folium.
7. **07-dashapp.py**: A fully interactive web dashboard built with Plotly Dash allowing real-time filtering of payloads and launch success rates.
8. **08_Machine_Learning_Prediction.ipynb**: Building and tuning predictive classification models (Logistic Regression, SVM, Decision Trees, and K-Nearest Neighbors) using GridSearchCV.

## Key Insights & Results
* **Best Performing Model**: All tuned classification models achieved a baseline accuracy score of **83.3%** on the test dataset, with **Support Vector Machine (SVM)** and **Decision Tree Classifier** showing optimal hyperparameter convergence via `GridSearchCV`.
* **Payload Impact**: Higher payload masses generally correlate with a higher success rate for first-stage landings.
* **Launch Site Success**: Operational success rates vary significantly by geographic location and proximity to coastlines.


## Tools & Libraries Used
* **Languages**: Python, SQL (SQLite)
* **Libraries**: Pandas, NumPy, Scikit-Learn, BeautifulSoup4, Requests
* **Visualization**: Matplotlib, Seaborn, Folium, Plotly Dash

