# NBA-MVP-Prediction
Machine Learning model to predict NBA MVP winners using 20+ seasons (2000-2025) of player data

# 🏀 NBA MVP Prediction — Machine Learning Project

![Python](https://img.shields.io/badge/Python-3.9+-blue)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.0+-orange)
![XGBoost](https://img.shields.io/badge/XGBoost-1.6+-green)

## 📌 Project Overview
An end-to-end Machine Learning pipeline to predict NBA MVP winners 
using 20+ seasons of player and team data (2000–2024).

Built by **Kelvin Attoh** — Data Science Student | Aspiring NBA Analytics Professional

---

## 🗂️ Dataset
- 14,491 player-season records across 20+ NBA seasons
- 11 datasets merged from NBA API, NBA website & Kaggle
- Severe class imbalance — only 25 MVP winners (1:539 ratio)

---

## ⚙️ Pipeline
1. Time-aware train/val/test split (no data leakage)
2. Feature scaling with StandardScaler
3. SMOTE oversampling inside each CV fold
4. Model training — Logistic Regression, Random Forest, XGBoost
5. Evaluation — F1, PR-AUC, ROC-AUC
6. SHAP interpretability

---

## 🏆 Results

| Model | CV Mean F1 | Test F1 |
|---|---|---|
| Logistic Regression | 0.4267 | 0.40 |
| **Random Forest** | **0.4833** | **1.00** |
| XGBoost | 0.4560 | 0.50 |

**Best Model: Random Forest**

---

## 💡 Key Finding
Scoring (pts_per_game) ranked **18th** in feature importance.
Top features: Win Shares, Offensive BPM, VORP — stats that 
measure team impact, not individual glory.

---

## 📈 Visualizations
![Top 10 MVP Candidates](visualizations/top10_mvp_candidates.png)
![SHAP Plot](visualizations/shap_bar_plot.png)

---

## 🛠️ How to Run
```bash
git clone https://github.com/YOUR_USERNAME/NBA-MVP-Prediction.git
cd NBA-MVP-Prediction
pip install -r requirements.txt
jupyter notebook notebooks/nba_mvp_prediction.ipynb
```

---

## 👤 Author
**Kelvin Attoh**
📍 Johnson City, TN
🎯 Aspiring NBA Data Scientist
🐂 Chicago Bulls Fan

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue)](YOUR_LINKEDIN_URL)
