# ⚽ Fintech Project: Predicting Football Players' Future Market Value

<p align='center'>
  <a href="https://github.com/yuvalmar16">Yuval Margolin</a> | 
  <a href="https://github.com/RavidGersh59">Ravid Gersh</a> | 
  <a href="https://github.com/ransela033">Ran Sela</a> | 
  <a href="https://github.com/yourlink-here">Yarden Nahum</a>
</p>

---

## 🧠 Project Overview

This project focuses on **predicting the future market value of professional football players** based on their physical attributes, technical skills, club affiliation, and historical performance data.

By using FIFA datasets from 2015 to 2023, we developed a machine learning pipeline that analyzes player features and forecasts their valuation **one year** and **two years** into the future.

---

## 📁 Files

| File | Description |
|:---|:---|
| `Fintech_Project_Code.ipynb` | Full notebook implementation — data cleaning, feature engineering, model training, evaluation, and visualization. |
| `Summary.pdf` | High-level project summary — feature selection logic, dataset details, modeling approach, and key conclusions. |
| `Detailed_Report.pdf` | In-depth technical report — modeling methodology, evaluation metrics, model comparisons, error analysis, and detailed results per player position. |

---

## 🎯 Objective

- Build a predictive system for estimating **players' future market value**.
- Analyze player data based on physical, technical, and club-related features.
- Compare multiple machine learning models to find the best-performing approach for valuation forecasting.

---

## 📊 Key Components

### 📂 Dataset

- **Source**:  
  [EA Sports FC 24 Complete Player Dataset on Kaggle](https://www.kaggle.com/datasets/stefanoleone992/ea-sports-fc-24-complete-player-dataset)

- **Data Range**:  
  Seasons 2015–2023.

- **Features Used**:  
  - Physical attributes: Age, Height, Weight
  - Performance skills: Pace, Passing, Shooting, Ball Control
  - Club information: Club rating, League prestige
  - Personal features: Nationality, Position, Work Rate
  - Special skills: Count of unique traits (e.g., flair, injury resistance)

- **Feature Engineering**:  
  - Interaction terms (e.g., Age × Stamina)
  - Polynomial features (e.g., Squared values for non-linear relations)
  - Categorical encoding
  - Aggregated special attributes

---

## 🔥 Models Used

- **Linear Regression**
  - Applied forward feature selection to optimize model simplicity and avoid overfitting.
  - Evaluated using Mean Absolute Error and Confidence Intervals.

- **Lasso Regression**
  - Used to perform feature selection automatically by applying L1 regularization.
  - Focused on retaining only the most impactful features for prediction.

- **Random Forest Regression**
  - Ensemble model leveraging multiple decision trees.
  - Ranked feature importance and improved generalization across noisy datasets.

---

## 📈 Evaluation

- Predicting **1-year** and **2-year** market value increases.
- Separate models trained for different player roles:
  - Goalkeepers
  - Defenders (Center Backs, Fullbacks)
  - Midfielders (Defensive and Attacking)
  - Strikers

- Metrics Analyzed:
  - Mean and Median residuals (prediction errors)
  - Confidence intervals
  - Sharpe and Sortino Ratios (for investment-style player selection)

- **Bonus Strategy**:
  - Invest in players predicted to increase value by 1.5× within a year.
  - Based on Linear Regression forecasts and top 9 selected features.

- Best performance was achieved with **Random Forest** and **Linear Regression with feature selection**, depending on the player group.

---

## 💡 Skills and Technologies

- Python 3.x
- Jupyter Notebook
- Pandas, NumPy
- Scikit-learn (Regression models, Random Forest, Feature Selection)
- Data Cleaning, Feature Engineering, Polynomial Transformation
- Exploratory Data Analysis (EDA)
- Model Evaluation Metrics (Sharpe Ratio, Sortino Ratio)

---

## 🤝 Contributors

- [Yuval Margolin](https://github.com/yuvalmar16)
- [Ravid Gersh](https://github.com/RavidGersh59)
- [Ran Sela](https://github.com/Ransela033)
- Yarden Nahum

---

## 📚 References

- ["Econometric Approach to Assessing the Transfer Fees and Values of Professional Football Players"](https://www.mdpi.com/2227-7099/10/1/4)
- ["Predict the Value of Football Players Using FIFA Video Game Data and Machine Learning Techniques"](https://ieeexplore.ieee.org/document/9721908)
- ["Explainable Artificial Intelligence Model for Identifying Market Value in Professional Soccer Players"](https://arxiv.org/abs/2311.04599)
- [Calcalist: "How Football Player Values Are Determined"](https://www.calcalist.co.il/sport/articles/0,7340,L-3745362,00.html)
- ["Valuing Soccer Players: Dynamics of an Online User Community"](https://www.emerald.com/insight/content/doi/10.1108/AAAJ-05-2022-5824/full/pdf)

---

