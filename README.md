# Supply Chain Delivery Delay Prediction
> *Can we predict whether a shipment will arrive late before it happens?*

**Author:** Dharshana | Data Science Student  
**Submitted for:** Digitivity Solutions — Data Science Internship Assessment | 2026

---

## Why This Dataset?

Supply chain logistics often face delays due to inefficient scheduling, operational bottlenecks, and high order volumes. Predicting delivery delays in advance allows companies to take proactive actions and improve operational efficiency.

This project develops a **machine learning model to predict late delivery risk** using supply chain data.

This is not just an academic exercise — it is a **proof-of-concept predictive analytics system for logistics operations.**

---

## Project Highlights

| What | Detail |
|---|---|
| Dataset | DataCo Smart Supply Chain Dataset (Kaggle) |
| Records | 180,519 supply chain transactions |
| Features | 40+ cleaned and engineered variables |
| Models trained | Random Forest, XGBoost |
| Best model | **Random Forest — 74.6% accuracy** |
| Visualizations | Distribution plots, heatmaps, learning curves |
| Goal | Predict late shipment risk |

---

## Results

| Model | Accuracy |
|---|---|
| Random Forest | **0.746** |
| XGBoost | 0.732 |

Random Forest slightly outperformed XGBoost and was selected as the **final model**.

---

## Key Findings

**1. Shipping schedule strongly influences delays**

Orders with tighter scheduled shipping timelines show higher late delivery risk.

**2. Order quantity and pricing affect delivery risk**

Large orders and higher-value transactions often require more logistics coordination.

**3. Shipping mode plays a role**

Certain shipping modes show higher delay probabilities compared to others.

**4. Tree-based models perform best**

Random Forest captured complex relationships between supply chain variables better than XGBoost.

---

## Feature Engineering

Several preprocessing steps were applied to improve model performance.

| Feature | Description |
|---|---|
| `order_day` | Extracted day from order date |
| `order_month` | Extracted month from order date |
| Encoded variables | Converted categorical features using one-hot encoding |
| Missing values | Filled using median imputation |

---

## Project Structure
```
digitivity/
│
├── notebooks/
│ └── supply_chain_prediction.ipynb
│
├── Data/
│ ├── DataCoSupplyChainDataset.csv
│ └── supply_chain_cleaned.csv
│
├── outputs/
│ ├── Confusion Matrix - Random Forest.png
│ ├── Distribution of Late Delivery Risk.png
│ ├── Distribution of Order Quantity.png
│ ├── Feature Correlation Heatmap.png
│ ├── Model Performance Comparison
│ └── model_learning_curve.png
│
└── README.md
```

---

## Setup & Installation

**1. Clone the repository**

git clone https://github.com/Dharshana-Git/Digitivity-SupplyChain
cd digitivity

**2. Install dependencies**

pip install pandas numpy matplotlib seaborn scikit-learn xgboost

**3. Run the notebook**

jupyter notebook notebooks/supply_chain_prediction.ipynb

---

## Notebook Structure

| Section | Description |
|---|---|
| 1. Problem framing | Business context |
| 2. Data loading | Dataset overview |
| 3. Data cleaning | Missing value handling |
| 4. EDA | Visual analysis |
| 5. Feature engineering | Feature transformation |
| 6. Model training | Random Forest & XGBoost |
| 7. Model comparison | Accuracy comparison |
| 8. Learning curve | Model training curve |
| 9. Conclusion | Insights and recommendations |

---

## Tech Stack

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-lightblue)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-green)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Plots-purple)
![ScikitLearn](https://img.shields.io/badge/ScikitLearn-MachineLearning-orange)
![RandomForest](https://img.shields.io/badge/RandomForest-Model-brightgreen)
![XGBoost](https://img.shields.io/badge/XGBoost-GradientBoost-red)

---

## Conclusion

This project demonstrates how machine learning can be applied to logistics data to predict delivery delays. Random Forest achieved the best performance with an accuracy of **74.6%**, making it the most suitable model for predicting late shipments.

Predictive systems like this can help logistics companies **anticipate delivery risks and improve operational efficiency.**

---

*"Predicting delays is not just about logistics — it's about improving customer experience."*
