
 🚀 SpaceX Falcon 9 Landing Prediction

# Project Overview
This project analyzes SpaceX Falcon 9 launch data to predict whether the first stage booster will successfully land. Since SpaceX reuses its first-stage boosters, a successful landing significantly reduces launch costs. This project explores what factors affect landing success and builds machine learning models to predict the outcome.

# Objectives
- Collect and clean SpaceX launch data using API and web scraping
- Perform Exploratory Data Analysis (EDA) using SQL and visualizations
- Build an interactive dashboard and geographic launch site map
- Train and compare multiple machine learning classification models
- Identify the best-performing model and the key factors driving success

# Tech Stack
- Language: Python,Machine learning
- Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Folium, Plotly Dash
- Database: SQL (SQLite/DB2)
- Tools:Jupyter Notebook, BeautifulSoup (web scraping), REST API

# Project Workflow
1. Data Collection — Retrieved launch data via SpaceX REST API and web-scraped historical data from Wikipedia
2. Data Wrangling— Cleaned missing values, engineered new features (e.g., landing outcome classification)
3. Exploratory Data Analysis (SQL & Visualization) — Queried and visualized trends across launch sites, payload mass, orbit types, and time
4. Interactive Visual Analytics— Built a Folium map of launch sites and a Plotly Dash dashboard
5. Predictive Analysis (Machine Learning)— Trained Logistic Regression, SVM, Decision Tree, and KNN models using GridSearchCV
6. Model Evaluation — Compared models using accuracy, feature importance, and ROC-AUC analysis

# Key Findings
- The Decision Tree Classifier performed best among all trained models
- Lighter payloads tend to have higher landing success rates
- Launch success rate improves over time as SpaceX gains experience
- KSC LC-39A recorded the highest number of successful launches
- Orbits GEO, HEO, SSO, and ES-L1 show the highest success rates

# Charts & Visualizations
- Model Accuracy Comparison— Bar chart comparing cross-validated accuracy of all 4 models
- Feature Importance Plot — Top 10 most influential features from the Decision Tree model
- ROC Curve Comparison — ROC curves and AUC scores for all trained models
- Launch Site Map — Interactive Folium map showing all SpaceX launch sites
- Payload vs Launch Site Scatter Plot — Relationship between payload mass and launch outcome
- Success Rate by Orbit Type— Visualization comparing success rates across different orbit types

# How to Run
1. Clone the repository
   git clone https://github.com/mamta3925-cse/spacex-falcon9-landing-prediction.git
2. Open the notebooks in Jupyter Notebook or JupyterLab
3. Each notebook installs its own required libraries at the top (e.g., !pip install <library>) — run those cells first before executing the rest

Author
[Mamta]

#Acknowledgements
This project was completed as part of the *IBM Data Science Professional Certificate*capstone project.
