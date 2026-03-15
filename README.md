<div align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python Badge"/>
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white" alt="Jupyter Badge"/>
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" alt="Scikit-Learn Badge"/>
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas Badge"/>
</div>

<br>

# ☕ Coffee Sales Analysis & Demand Forecasting

> **A comprehensive Data Pipeline and Machine Learning framework designed to optimize retail coffee operations by predicting demand surges.**

## 📖 Project Overview
Retail coffee demand is highly volatile, with extreme morning rushes causing significant operational bottlenecks. If Average Service Time (AST) exceeds 3 minutes, queue abandonment rises exponentially, resulting in lost daily revenue. 

This project transforms raw point-of-sale transaction logs into actionable, predictive forecasting models. By utilizing **Feature Engineering** (cyclical time encoding) and **Random Forest Ensembles**, this pipeline anticipates demand spikes up to 7 days in advance—shifting the operational mindset from reactive to proactive.

---

## 🚀 Key Technical Achievements
- **Robust Data Pipeline**: Ingested and optimized 89K+ transaction records, utilizing specific `dtypes` (`float32`, `category`) to minimize the initial memory footprint.
- **Trigonometric Feature Engineering**: Overcame linear time limitations by applying Sine and Cosine transformations to 24-hour cycles, mapping contextual behavioral flags (e.g. `is_morning_rush`).
- **Time-Series ML (Random Forest)**: Built a 300-estimator tree ensemble utilizing a strict sequential train/test split to prevent catastrophic future-data leakage.
- **Measurable ROI**: The model reduced Mean Absolute Error (MAE) by **34%** (from 14.2 cups to 9.4 cups), directly trimming perishable waste and recouping an estimated **$700/mo** in lost revenue.

---

## 📁 Repository Structure
```text
├── 📄 Task1_Coffee_Sales_Analysis.ipynb    # Core Machine Learning & Analysis Notebook
├── 📄 CoffeeSalesReport.pdf                # Executive Level Final Slide Deck
├── 📄 Coffee Sales Analysis Pdf.pdf        # Detailed Walkthrough Document
├── 📄 Task1_Coffee_Sales_PPT.html          # Interactive Web Presentation
└── 📄 index.csv (Not tracked)              # Raw Transaction Data (Local Only)
```

## 🛠️ Tech Stack & Methods
* **Language:** Python
* **Analytics & Manipulation:** `pandas`, `numpy`, `scipy`
* **Machine Learning:** `scikit-learn` (RandomForestRegressor, Z-Score Statistical Filtering)
* **Visualization:** `matplotlib`, `seaborn`

## 📊 Visualized Insights
A structural analysis of the transaction volume revealed a clear **Bimodal Surge Pattern**:
1. **The Commuter Surge (07:00 - 09:30):** Extreme transaction velocity targeting low-complexity items (drip coffee). Operating principle: *Throughput Maximization*.
2. **The Social Block (13:00 - 15:00):** Lower velocity, higher Average Transaction Value (ATV). Operating principle: *Menu Agility*.

## ⚙️ How to Run
1. Clone the repository: `git clone https://github.com/dayaxi2005-hub/Task1_Coffee_Sales_Analysis.git`
2. Open the notebook in your preferred environment (Jupyter, VSCode, Google Colab).
3. Ensure exact Python requirements are satisfied:
   `pip install pandas==2.1.0 numpy==1.25.0 matplotlib==3.7.0 seaborn==0.12.0 scikit-learn==1.3.0 scipy==1.11.0`
4. Execute cells linearly.

---
*Authored by Finance Analyst as a Demonstration of Advanced Market Modeling.*
