# 🛒 Promotion Profitability Predictor (FMCG – UAE Market) 🇦🇪  

### Predicting Profitable Promotions Before They Launch

---

## 🧠 Overview

This project applies **Binary Classification** to historical **sales and promotion data** in the **Fast-Moving Consumer Goods (FMCG)** sector.  

The objective is to **predict whether a proposed promotional campaign will be financially profitable** — i.e., whether it will **break even** before launch — to **protect marketing budgets** and **maximize ROI**.

The model focuses on **minimizing risk (False Positives)** rather than maximizing total capture (Recall).  
This aligns with real-world business needs: preventing unprofitable campaigns is more important than finding every possible good one.

---

## 💼 Business Problem & Goal

| Category | Description |
|-----------|-------------|
| **Problem** | High rate of **False Positives** in promotion planning — campaigns predicted to succeed but failing to generate sufficient Incremental Sales Lift to cover costs. |
| **Goal** | Achieve a minimum of **80% Precision** in predicting promotional success to ensure that **8 out of 10 recommended campaigns** are profitable. |
| **Target Variable** | `Success` / `Failure` (`1` or `0`) — defined by comparing **Incremental Sales Lift** to the **Breakeven Volume (BEV)** threshold (40 units). |

---

## ❓ Business Questions Answered

This model empowers **FMCG marketing managers** with **data-driven decision support**:

1. **Profitability Forecast**  
   → *Will this promotion type, depth, and duration achieve the Breakeven Volume to cover the AED 40 cost?*

2. **Risk Assessment**  
   → *What is the probability of success?*  
   → *Should we only launch campaigns with a predicted success probability above 70%?*

3. **Driver Identification**  
   → *Which features (e.g., BOGO, Hypermarket Format) drive profitability?*  
   → *Which are the biggest risk factors?*

---

## 🧰 Technology Stack

| Component | Technology | Purpose |
|------------|-------------|----------|
| **Language** | Python | Core development and modeling |
| **Data Processing** | Pandas, NumPy | Synthetic data generation, feature engineering, BEV calculation |
| **Modeling** | Scikit-learn | Logistic Regression, train/test split, model tuning |
| **Evaluation & Visualization** | Matplotlib, Seaborn | Confusion Matrix visualization, Feature Importance plots |
| **Deployment (Planned)** | Power BI / Tableau | Interactive dashboard for scenario planning |

---

## 📊 Key Project Findings & Impact

### 🎯 Precision Over Recall  
- Adjusted the **classification threshold** to achieve **≥ 80% Precision**, ensuring higher profitability confidence.  
- Accepted reduced Recall to minimize **budget risk** (missed opportunities preferred over failed promotions).

### 💡 Feature Drivers  
- **Positive Impact:**  
  - `BOGO Promotions`  
  - `Hypermarket Store Format`  
- **Negative Impact:**  
  - `Simple Discount (15%)` → strong negative coefficient → *avoid frequent use.*

### 🧾 Business Impact  
- **Risk Mitigation:** Prevents unprofitable campaign launches.  
- **Budget Efficiency:** Ensures marketing spend drives measurable ROI.  
- **Decision Transparency:** Explains *why* promotions succeed or fail via interpretable coefficients.

---

## ⚙️ Model Evaluation Metrics

| Metric | Description | Goal |
|--------|--------------|------|
| **Precision** | % of predicted profitable promotions that actually are | ≥ 80% |
| **Recall** | % of all profitable promotions correctly identified | Secondary |
| **F1-Score** | Harmonic mean of Precision & Recall | Balanced metric |
| **Confusion Matrix** | Visual diagnostic tool | Evaluate trade-offs |

---

## 🚀 Future Work

- **Interactive Dashboard:** Real-time promotion simulations via Power BI/Tableau.  
- **Model Upgrade:** Test ensemble models (XGBoost, Random Forest) for better recall without hurting precision.  
- **AutoML Pipeline:** Integrate MLOps for automated retraining as new sales data arrives.  
- **Business API:** Expose the predictor through a RESTful API for integration with retail ERP systems.

---

## 🧩 Repository Structure


---

## 🏁 Key Takeaway

> “By prioritizing **precision over recall**, this model shifts marketing from guesswork to grounded, data-backed decision-making — enabling UAE FMCG brands to launch only those promotions that truly pay off.”

---

### 👤 Author
**Mohamed Nizzad**  
_Data Science & AI | FMCG Analytics | MLOps Enthusiast_  
📧 [LinkedIn](https://www.linkedin.com/in/mohamednizzad) | 🌐 [Portfolio](#)

---

