# 🧪 A/B Test Analysis: Landing Page Conversion

Statistical analysis of an A/B test to determine whether a new landing page design has a significant impact on conversion rate.

---

## 📋 Project Overview

An e-commerce company tested a redesigned landing page. The goal was to determine whether the new design statistically significantly affects the conversion rate and whether it should be rolled out to all users.

**Hypotheses:**
- **H₀:** The new design has no effect on conversion rate — the difference between groups is random
- **H₁:** The new design changed the conversion rate in either direction
- **Significance level:** α = 0.05

---

## 🔧 What I Did

- **Data cleaning** — removed duplicate users (3,894 records) and rows with mismatched group/page assignments (2,044 records)
- **Exploratory data analysis** — assessed group sizes and conversion rates per group
- **Statistical testing** — applied a two-proportion z-test and interpreted the p-value

---

## 📊 Results

| Group | Users | Conversions | Conversion Rate |
|-------|-------|-------------|-----------------|
| Control (old page) | 144,226 | 17,349 | 12.03% |
| Treatment (new page) | 144,314 | 17,134 | 11.87% |

**p-value = 0.195** — above the 0.05 threshold

---

## 💡 Conclusion

No statistically significant evidence was found that the new design affects conversion rate. The 0.16 p.p. difference between groups is likely due to random variation.

**Recommendations:**
1. Verify that the test ran for its full planned duration and was not stopped early (peeking problem)
2. Calculate the required sample size via power analysis before the next test
3. Run a follow-up test with a properly calculated sample size

---

## 🛠️ Stack

`Python` `pandas` `numpy` `statsmodels`

---

## 📂 Data Source

[A/B Testing Dataset](https://www.kaggle.com/datasets/zhangluyuan/ab-testing) — Kaggle

---

## 📅 Status

✅ Completed — June 2026
