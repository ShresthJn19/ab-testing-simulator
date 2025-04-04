# 📊 A/B Marketing Test – Impact of Ad Exposure on Conversion

This project analyzes the impact of an online ad campaign on user conversion using a clean A/B testing approach. By comparing users who saw ads (test group) to those who saw a public service announcement (control group), we evaluated the effectiveness of the ad campaign and its contribution to revenue.

---

## 🎯 Objective

- Determine if showing ads increases user conversion
- Measure the size of the uplift and test if it’s statistically significant
- Estimate incremental revenue generated by the ad campaign

---

## 📦 Dataset Overview

- **Source:** Kaggle – Marketing A/B Testing
- **Observations:** 588,101 users
- **Key Features:**
  - `test group`: 'ad' or 'psa'
  - `converted`: True/False (target)
  - `total ads`: Number of ads shown
  - `most ads day`: Day with most ad exposure
  - `most ads hour`: Peak ad hour

---

## 🔍 Analysis Workflow

### 1️⃣ Conversion Rate Comparison

- Grouped users by `test group`
- Calculated conversion rates:
  - **Ad Group:** ~2.55%
  - **PSA Group:** ~1.78%
- Resulted in a **43% relative lift** from showing ads

### 2️⃣ Statistical Significance (Z-test)

- Performed a **proportions Z-test** using `statsmodels`
- Result:
  - **Z-stat:** ~7.37
  - **p-value:** < 0.000
  - ✅ **Statistically significant difference**

### 3️⃣ Revenue Estimation

- Assumed **Average Order Value = $50**
- Estimated **incremental revenue** from ad-driven conversions:
  - ➕ ~$217,149.11

### 4️⃣ Ad Exposure Analysis

- Visualized ad exposure (boxplot: `total ads` vs `converted`)
- Found:
  - Converted users saw **more ads**
  - Most users saw fewer than 100 ads
  - Outliers present, but not driving the main result

---

## 📈 Key Takeaways

- ✅ The ad campaign **significantly improved conversion**
- ✅ Statistical evidence confirms the uplift is **real, not random**
- ✅ Users who converted were typically exposed to more ads
- ✅ Ads likely drove an additional **$217K+ in revenue**

---

## 🛠️ Tools Used

- Python (pandas, seaborn, matplotlib)
- `statsmodels` (Z-test for proportions)
- Jupyter Notebook

---

## 📊 Metrics Summary

| Metric                | Value        |
| --------------------- | ------------ |
| Conversion Rate (Ad)  | 2.55%        |
| Conversion Rate (PSA) | 1.78%        |
| Lift                  | 43.3% ↑      |
| p-value               | 0.0000 ✅    |
| Extra Revenue         | ~$217,149.11 |
