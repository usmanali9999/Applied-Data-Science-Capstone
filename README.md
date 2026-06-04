# IBM Applied Data Science Capstone Project

An end-to-end data science pipeline built to predict the landing success of SpaceX Falcon 9 rocket first-stage boosters, maximizing cost-efficiencies for commercial aerospace launches.

## 📌 Project Overview
This repository contains the complete portfolio framework for the **IBM Applied Data Science Capstone** curriculum. The project spans data ingestion via web scraping and REST APIs, relational database management using SQL, interactive geospatial visualization, web-app dashboard deployment, and hyperparameter-tuned machine learning classification algorithms.

### 🚀 Core Data Pipeline Phases
1. **Data Collection & Extraction**: Gathering launch logs using the SpaceX REST API and scraping historical Wikipedia tables using `BeautifulSoup4`.
2. **Data Wrangling & Processing**: Handling null parameters, feature engineering categorical metrics using One-Hot Encoding, and flattening raw payloads.
3. **Exploratory Data Analysis (EDA)**: Executive data analysis utilizing SQL queries and relational visualization plots.
4. **Geospatial Mapping**: Isolating launch pad coordinates, safety distances, and landing failure/success metrics using interactive map overlays.
5. **Interactive Dashboard App**: Deploying a live analytics control panel featuring structural charts and reactive filter selectors.
   
<br>

<div align="center">
  <div style="display: inline-block; vertical-align: middle; margin-right: 20px;">
    <p><b>Launch Site Success Proportions</b></p>
    <img src="pie_chart.png" width="440">
  </div>
  <div style="display: inline-block; vertical-align: middle;">
    <p><b>Payload Mass vs. Success Correlation</b></p>
    <img src="scatter_plot.png" width="490">
  </div>
</div>

<br>

 





7. **Predictive Modeling (ML)**: Training, tuning, and bench-testing four separate categorization algorithms to declare the optimal landing predictor model.

---

## 📂 Repository Structure
```text
├── .gitignore                               # System files to ignore in Git
├── 01_data-collection-api.ipynb             # Fetching raw SpaceX API data array streams
├── 02_webscraping.ipynb                     # Web scraping launch records via BeautifulSoup
├── 03_Data wrangling.ipynb                  # Data cleaning and feature engineering phase
├── 04-eda-with-sql.ipynb                    # Analyzing dataset patterns using SQL queries
├── 05_edadataviz.ipynb                      # Exploratory data visualizations with Seaborn
├── 06_launch_site_location.ipynb            # Geospatial mapping coordinates using Folium
├── 07-dashapp.py                            # Interactive web-app layout dashboard script
├── 08_Machine_Learning_Prediction.ipynb     # ML model training and hyperparameter tuning
├── 09_DataScience_Capstone_Presentation.pdf # Executive summary slide presentation
├── LICENSE                                  # Open-source distribution parameters
├── README.md                                # Comprehensive documentation handbook
└── requirements.txt                         # Complete project software package dependencies
```

---

## 🛠️ Built With
* **Python 3** - Underlying programming runtime.
* **Scikit-Learn** - Machine learning classification models & GridSearchCV tuning.
* **Plotly Dash** - Dynamic data application framework environment.
* **Folium** - Interactive HTML geospatial map visualization layers.
* **Pandas / NumPy** - Matrix manipulations and structured data processing pipelines.
* **BeautifulSoup4 / Requests** - Web scraping tools and REST API parsing pipelines.

---

## 🚀 Getting Started

### Prerequisites
Configure your local environment automatically by installing all the tracked project library dependencies directly via the configuration file:
```bash
pip install -r requirements.txt
```

### Execution Steps
1. Clone this repository to your local system environment:
   ```bash
   git clone https://github.com/usmanali9999/Applied-Data-Science-Capstone.git
   cd Applied-Data-Science-Capstone
   ```
2. Start the interactive workspace environment:
   ```bash
   jupyter notebook
   ```
3. Run the development notebooks in sequence (`01_data-collection-api.ipynb` through `08_Machine_Learning_Prediction.ipynb`) to replicate the data insights pipeline.
4. Launch the live dashboard visualization application locally:
   ```bash
   python 07-dashapp.py
   ```

---
## 📊 Predictive Machine Learning Results
The performance of each hyperparameter-tuned machine learning algorithm was assessed using classification accuracy scores:


| Classification Model | Accuracy Score (Training Data) | Best Parameters Discovered |
|---|---|---|
| **Logistic Regression** | 84.6% | `C: 0.01`, `penalty: l2`, `solver: lbfgs` |
| **Support Vector Machine (SVM)** | 84.6% | `C: 1.0`, `kernel: rbf`, `gamma: scale` |
| **Decision Tree Classifier** | 84.6% | `criterion: gini`, `max_depth: 4`, `splitter: best` |
| **K-Nearest Neighbors (KNN)** | 84.6% | `n_neighbors: 10`, `algorithm: auto`, `p: 2` |

*Note: All optimized classification architectures yielded a tied baseline performance matrix accuracy across validation sets, heavily driven by the initial engineered feature profiles.*

---

## 📄 License
Distributed under the MIT License. See `LICENSE` for more details.
