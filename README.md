# 📊 A/B Marketing Test – Conversion Impact of Ad Exposure

This project analyzes a marketing A/B test to evaluate whether displaying ads increases user conversion. Using statistical methods and visual analysis, we compare conversion behavior between users shown ads (test group) and those shown public service announcements (control group).

---

## 🎯 Objective

- Determine if exposure to ads leads to a higher conversion rate
- Measure the magnitude of improvement (lift)
- Test whether the improvement is statistically significant
- Estimate potential revenue impact

---

## 🧾 Dataset Summary

- **Users:** 588,101
- **Groups:** `ad` (test) vs `psa` (control)
- **Target:** `converted` (True/False)
- **Features:**
  - `total ads`: Number of ads shown
  - `most ads day`: Day with highest ad exposure
  - `most ads hour`: Hour with highest ad exposure

Source: [Marketing A/B Testing Dataset on Kaggle](https://www.kaggle.com/datasets/faviovaz/marketing-ab-testing)

---

## 📈 Analysis Overview

### ✅ Conversion Comparison

- Calculated conversion rates for `ad` and `psa` groups
- Found uplift (relative increase) from ad exposure

### ✅ Hypothesis Testing

- Used **Z-test for proportions** to evaluate statistical significance
- Interpreted Z-stat and p-value to validate results

### ✅ Revenue Estimation

- Estimated additional revenue using:
  - Extra conversions driven by ads
  - Assumed average order value ($50)

### ✅ Visualizations

- Boxplot of `total ads` vs conversion status
- Showed that higher ad exposure correlates with higher conversion likelihood

---

## 📊 Key Results

- **Conversion Lift from Ads:** +8.6% (approx)
- **Statistical Significance:** p < 0.001 → strong evidence
- **Estimated Revenue Uplift:** ~$180,000 from incremental conversions
- **Insight:** Converted users in ad group saw more ads (higher median exposure)

---

## 🛠️ Tools & Libraries

- Python (pandas, seaborn, matplotlib)
- `statsmodels` (for Z-test)
- Jupyter Notebook

---

## 🧠 Takeaway

This project demonstrates the full A/B testing workflow:

- Clear hypothesis framing
- Real conversion metrics
- Statistical validation
- Business impact estimation

It reflects how data science drives actionable marketing decisions.
