# 🌩️ Hailstorm ML Analysis (2000–2024)

[![Open In Colab](https://colab.research.google.com/drive/1V9QuS41_Fy1OeRbiiuQHQnDTa_keYtEl)](https://colab.research.google.com/github/[YOUR_GITHUB_USERNAME](https://github.com/AniketSaha17)/Hailstorm-ML-Analysis/blob/main/notebooks/hailstorm_analysis.ipynb]

This repository contains the analysis and machine learning classification of hailstorm events over Kolkata and surrounding regions, based on meteorological data from 2000–2024.

## 📌 Project Overview
The study identifies hailstorm patterns using weather parameters and machine learning.  
Key steps include:
- Data collection from Kaggle datasets (2000–2024)
- Preprocessing & feature engineering (temperature, rainfall, humidity, CAPE, etc.)
- Exploratory Data Analysis (EDA) with visualizations
- Machine learning models for hailstorm classification:
  - Decision Tree, Random Forest, SVM, XGBoost
- (Optional/Planned) Spatiotemporal analysis using GIS overlays

## 🔬 Methods
- **Programming:** Python 3.11 (Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn)
- **Visualization:** Histograms, boxplots, heatmaps, feature importance plots
- **Evaluation:** Accuracy, Precision, Recall, F1-score, ROC-AUC

## 📊 Key Results
- **Random Forest** and **XGBoost** achieved the highest accuracy in classifying hail events.
- Feature importance analysis highlighted **CAPE, precipitation intensity, and humidity** as dominant predictors.
- Pre-monsoon (March–May) emerged as the most hail-prone period.

## 📂 Repository Structure

Hailstorm-ML-Analysis/
├── data/ # place raw data here (not tracked)
├── figures/ # exported plots (tracked)
├── models/ # saved models (.pkl) - consider Git LFS
├── notebooks/ # Colab / Jupyter notebooks
├── paper/ # manuscript and references (optional)
├── src/ # reusable python scripts (optional)
├── README.md
├── requirements.txt
└── .gitignore

# 📂 Data Guide

This project uses publicly available weather data from Kaggle.  
Raw CSV files are **not included in this repository** due to size and licensing restrictions.

## 🔗 Dataset Source
- Sourasish02. (2024). *Kolkata Weather Data (2000–2024)* [Data set]. Kaggle.  
  👉 https://www.kaggle.com/datasets/sourasish02/kolkata-weather-data-2000-2024

## 📥 How to Use
1. Download the dataset from the Kaggle link above.  
2. Place the extracted CSV files into the `data/` folder of this repository.  
   Example:
Hailstorm-ML-Analysis/
├── data/
│ ├── weather.csv
│ └── Daily_weather_data.csv

3. Run the analysis notebook (`notebooks/hailstorm_analysis.ipynb`) — it will automatically load the CSVs from `data/`.


## ▶️ How to Run (Colab)
1) Open `notebooks/hailstorm_analysis.ipynb` in Google Colab  
2) Upload datasets to `/content/data/` or mount Google Drive  
3) Install dependencies:
```bash
```
pip install -r requirements.txt
4. Run cells to reproduce preprocessing, training, and plots.

# Core
pandas==2.2.2
numpy==1.26.4

# Visualization
matplotlib==3.9.0
seaborn==0.13.2

# Machine Learning
scikit-learn==1.5.0
xgboost==2.0.3
imbalanced-learn==0.12.2

# Jupyter/Colab
notebook
jupyter


## ⚠️ Note
- This repository does **not redistribute** raw data. Please follow Kaggle’s license terms when downloading and using the dataset.  
- If you use this dataset in academic work, cite it appropriately:  
> Sourasish02. (2024). *Kolkata Weather Data (2000–2024)* [Data set]. Kaggle. https://www.kaggle.com/datasets/sourasish02/kolkata-weather-data-2000-2024

## 📈 Example Figures
- Average temperature and rainfall trends (2000–2024)
- Year-over-year % change in weather parameters
- Confusion matrices of ML models
- ROC curves comparison
- Feature importance (Random Forest & XGBoost)

🔗 References

Indian Meteorological Department (IMD). (2024). Doppler Weather Radar Network Data. https://mausam.imd.gov.in/
ERA5 Climate Data. (2024). ECMWF Reanalysis v5. Copernicus Climate Change Service (C3S). https://cds.climate.copernicus.eu/
(Full reference list available in paper draft)

📜 Data & Licensing

Do not commit Kaggle raw datasets unless the license permits redistribution.
Provide links/instructions to download the data instead.

## Acknowledgements
KPRIET support and collaboration with faculty (methods & review).

---

✨ **Author:** [Aniket Saha] (Associate Technical Lead, KPRIET)  
🔎 **Areas of Interest:** Data Analytics, Data Science, Machine Learning  
📬 Feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/aniket-saha-7620301b3/)

