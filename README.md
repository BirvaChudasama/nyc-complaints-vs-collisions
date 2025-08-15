# nyc-complaints-vs-collisions
Analysis of historical and real-time NYC 311 complaints and traffic collisions to uncover patterns, correlations, and trends. Includes descriptive analytics, clustering, time-series forecasting, and live API integration for traffic risk insights. Built with Python, Jupyter, Pandas, and visualization tools
# NYC 311 Complaints & Motor Vehicle Collision Analysis 🚦📊

##   Project Overview
This project analyzes the relationship between **NYC 311 service complaints** and **motor vehicle collisions** to identify high-risk zones, patterns, and trends.  
It integrates **historical datasets** with the **NYC Open Data 311 API** to enable **real-time predictive modeling** and **risk alert simulations** for smarter urban safety management.

##  Objectives
- Identify **complaint–crash correlations** across NYC boroughs.
- Forecast **complaint and crash volumes** using **SARIMAX** & **Facebook Prophet**.
- Map **collision & complaint hotspots** using geospatial analysis.
- Simulate **real-time risk alerts** from API data.
- Provide insights to improve **traffic safety** and **response planning**.

##  Data Sources
1. **Motor Vehicle Collisions – Crashes** (NYC Open Data CSV)
2. **311 Service Requests** (NYC Open Data API)
3. Weather & external variables (optional future expansion)

## 🔍 Key Features
- **Data Integration**: Combines CSV datasets and live API calls.
- **Time Lag Analysis**: Measures complaint spikes before crashes.
- **Geospatial Mapping**: Borough-level heatmaps & location clustering.
- **Predictive Modeling**: SARIMAX for trend forecasting, Prophet for seasonal patterns.
- **Real-Time Simulation**: Streams API data into forecasts.
- **Visualization Dashboard**: Power BI / Tableau interactive reports.

## 🛠️ Tech Stack
- **Languages**: Python, SQL
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Statsmodels, Prophet, Folium, GeoPandas, Requests
- **Visualization**: Power BI, Tableau, Matplotlib
- **API**: NYC Open Data 311 API
- **Environment**: Jupyter Notebook, Virtual Environment (nyc_env)

## 📊 Analytical Approach
### 1. Descriptive Analytics
- Complaint–crash correlation heatmaps
- Top boroughs by collision density
- WordClouds of frequent complaint types

### 2. Unsupervised Learning
- **K-Means / DBSCAN** clustering for hotspot detection
- Grouping boroughs by complaint–collision patterns

### 3. Time Series Forecasting
- SARIMAX for borough-level crash trends
- Prophet for long-term complaint trends
- Evaluation metrics: RMSE, MAPE

### 4. Real-Time Alert Simulation
- Pulls API data periodically
- Updates forecast models
- Generates simulated alerts

## 📌 System Architecture

[Data Sources: CSV + API] --> [Data Cleaning & Preprocessing] --> [Feature Engineering] -->
[Analytics & Modeling: SARIMAX / Prophet / Clustering] --> [Visualization & Dashboard] --> [Real-Time Alerts]


## 📈 Results & Insights
- Found a strong correlation between **traffic signal complaints** and collision hotspots.
- Time-lag patterns suggest targeted intervention windows.
- Seasonal & weekday trends help optimize resource allocation.
- Forecast models demonstrate >80% accuracy on validation sets.


Clone the repository
https://github.com/BirvaChudasama/nyc-complaints-vs-collisions/tree/main

Create a virtual environment
		python -m venv nyc_env

# Activate (Mac/Linux)
source nyc_env/bin/activate

# Activate (Windows)
nyc_env\Scripts\activate

     1 .Install dependencies

	pip install -r requirements.txt

    2  Run Jupyter notebooks

Run the notebooks in the following order to process data, fetch live updates, generate insights, and prepare dashboards.

1. **Combine & Clean Data**

   - `combine_csv_all.ipynb` → Merges and cleans historical collision and complaint datasets.

2. **Live 311 Complaint Data**

   - `comlaint_nyclive.ipynb` → Connects to the **NYC 311 API** and fetches **live complaint data** for integration with historical datasets.

3. **Historical Insights & Analysis**

   - `NYC Collision_historical_insight.ipynb` → Performs **descriptive analytics**, correlation analysis, and predictive modeling using historical data.

4. **Dashboard Preparation**

   - `dashboard_web.ipynb` → Prepares data and visual outputs for dashboards.

5. **View dashboards**
Open the .pbix file in Power BI

<img width="1505" height="847" alt="image" src="https://github.com/user-attachments/assets/08ca58bc-d0ce-4b6f-b044-a9e8052d2db1" />

<img width="1435" height="811" alt="image" src="https://github.com/user-attachments/assets/de84df1b-8c92-4e6d-a3d1-2303cede41b1" />

<img width="1423" height="813" alt="image" src="https://github.com/user-attachments/assets/0511a01d-0985-4d79-855b-535e02244089" />



Open the .twb file in Tableau

👩‍💻 Author

Birva  PankajKumar Chudasama

🎓 Post Graduate Certificate in Big data Analysis – Georgian College

📍 Based in Ontario, Canada

💼 Interests:  Data Analytics, Machine Learning, 

🔗 LinkedIn Profile :https://www.linkedin.com/in/birva-chudasama





