# Uber-Driver-Activation-A/B-Testing-Python-Pandas-Statistics
# 🚗 Uber Driver Activation — A/B Testing & Onboarding Analysis

## 📌 Project Overview

This project analyzes **54,681 driver onboarding records** to evaluate whether a redesigned Uber Partner App improves driver activation. The analysis combines **Exploratory Data Analysis, A/B Testing, Statistical Analysis, and Machine Learning** to identify factors influencing successful driver onboarding.

The primary KPI is **Driver Activation Rate**, defined as the percentage of signed-up drivers who complete their first ride.

---

## 🎯 Business Objective

Evaluate the effectiveness of the redesigned driver app and identify opportunities to:

* Increase driver activation
* Reduce onboarding friction
* Improve onboarding completion speed
* Identify high-performing acquisition channels
* Determine which driver characteristics influence activation

---

## 🛠️ Tools & Technologies

* **Python**
* **Pandas & NumPy**
* **Matplotlib & Seaborn**
* **Scikit-learn**
* **Statistical Testing**

  * Two-Proportion Z-Test
  * Chi-Square Test
  * One-Way ANOVA
  * Spearman Correlation
* **Jupyter Notebook / Google Colab**

---

## 🔍 Analysis Workflow

### 1. Data Cleaning

* Checked missing values and duplicates
* Converted date columns into appropriate datetime formats
* Handled missing vehicle information using `"Unknown"`
* Created onboarding duration features

### 2. Exploratory Data Analysis

Analyzed:

* Signup channels and platforms
* Experiment group distribution
* Driver activation
* Vehicle characteristics
* Signup trends
* City-level patterns
* Onboarding funnel performance

### 3. Feature Engineering

Created key features including:

* `vehicle_age`
* `signup_to_bgc`
* `bgc_to_vehicle`
* `signup_to_first_ride`
* `first_ride_completed`

---

## 📊 Key Findings

### A/B Test Results

| Metric                 |    Control |  Treatment |
| ---------------------- | ---------: | ---------: |
| Driver Activation Rate | **11.17%** | **11.27%** |

The two-proportion Z-test produced a **p-value ≈ 0.70**, indicating that the difference was **not statistically significant**. Therefore, the redesigned app did not demonstrate a meaningful overall activation uplift.

### Signup Channel Analysis

A Chi-Square test identified a statistically significant relationship between signup channel and driver activation.

* **Referral:** ~20% activation
* **Organic:** ~9% activation
* **Paid:** ~6% activation

Referral showed the strongest activation performance, while Paid generated the highest signup volume but the lowest activation rate.

### Onboarding Funnel

Average onboarding durations:

* Signup → Background Check: **~6 days**
* Background Check → Vehicle Upload: **~1.6 days**
* Signup → First Ride: **~1.35 days**

Spearman correlation between Signup-to-BGC and BGC-to-Vehicle time was **0.25**, indicating a weak-to-moderate positive relationship.

### Machine Learning

A **Random Forest Classifier** was used to identify important predictors of driver activation.

Key predictors included:

* Vehicle Age
* BGC-to-Vehicle Upload Time
* Signup-to-BGC Time

The model achieved approximately **93% accuracy** in the project analysis.

---

## 💡 Business Recommendations

1. **Reduce onboarding friction** by simplifying vehicle/document uploads.
2. **Improve Paid acquisition quality**, as Paid had high signup volume but low activation.
3. **Strengthen Referral programs** because of their higher activation rate.
4. **Use targeted reminders** for drivers experiencing onboarding delays.
5. **Investigate city-level differences** and test targeted interventions.
6. **Run a follow-up A/B test** before considering a broader rollout.

---

## 🚦 Final Recommendation

**Decision: Pivot → Iterate, Segment & Retest**

The redesigned app should **not be rolled out globally yet**, because the observed activation improvement was not statistically significant. However, there is also no evidence of a major negative impact, so a complete rollback is unnecessary.

The recommended approach is to improve high-friction onboarding steps, evaluate specific driver segments, and conduct a follow-up controlled experiment before making the final rollout decision.

---

## 📁 Project Structure

```text
Uber-A-B-Testing/
│
├── Uber_A_B_Testing_Project.ipynb
├── Uber_A_B_Testing.xlsx
├── Uber_A_B_Testing_Tasks.docx
└── README.md
```

---

## 📈 Skills Demonstrated

**Data Analysis | Data Cleaning | EDA | Feature Engineering | A/B Testing | Hypothesis Testing | Statistical Analysis | Machine Learning | Business Insights | Data-Driven Recommendations**
