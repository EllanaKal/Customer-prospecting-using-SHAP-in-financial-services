# Customer-prospecting-using-SHAP-in-financial-services

This project demonstrates how a financial institution can use machine learning and SHAP (SHapley Additive exPlanations) to predict which customers are most likely to buy a new **digital financial product**, such as an online investment account.

---

## 🧠 Objective
To build a transparent and explainable model that helps marketing teams target high-potential customers based on data-driven insights.

---

## ⚙️ Project Steps

1. **Data Generation / Loading**  
   Synthetic customer data is generated for demonstration:
   - Age  
   - Tenure  
   - Credit Score  
   - Average Balance  
   - Digital Engagement (# of logins per month)  
   - Previous Product Purchase  
   - Income  

2. **Model Building**  
   - Train an **XGBoost classifier** to predict purchase likelihood.
   - Evaluate with metrics like AUC, Accuracy, and Recall.

3. **Explainability with SHAP**  
   - Compute global and local SHAP values.
   - Visualize:
     - **SHAP Summary Plot** → Key drivers of model predictions.
     - **Waterfall Plot** → Individual customer-level explanations.

4. **Business Use**  
   - Identify top customer segments with high predicted probability.
   - Explain model decisions to marketing and compliance teams.

---

## 📊 Results Interpretation

| Feature | Typical Impact |
|----------|----------------|
| **Digital_Engagement** | Strong positive influence — frequent app users buy more digital products. |
| **Avg_Balance** | Higher balances → higher likelihood of purchase. |
| **Previous_Purchase** | Customers with past product engagement are more responsive. |
| **Age** | Older customers show slightly lower digital adoption. |

---

## 📈 Example Visuals
- `images/shap_summary.png` — Global feature importance.  
- `images/shap_waterfall.png` — Local prediction explanation.

---

## 🧩 Tools & Libraries
- Python 3.x  
- XGBoost  
- scikit-learn  
- SHAP  
- matplotlib  

