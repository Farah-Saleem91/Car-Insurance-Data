
![dataset-cover](https://github.com/user-attachments/assets/ec624141-2d46-48d9-a66a-3602ae1b9b8b)
# 🚗 Car Insurance Data Analysis

## 📘 Project Overview
This project explores and analyzes a car insurance dataset to identify the key factors that influence insurance outcomes such as claims or risk levels.
The analysis includes data cleaning , preprocessing, exploratory data analysis (EDA), feature importance evaluation, and business interpretation of results.

## 🎯 Objectives

-Understand relationships between driver, vehicle, and behavioral features.

-Identify which variables most strongly affect the insurance outcome (e.g., claim occurrence).

-Provide actionable business insights that align with real-world insurance logic.

-Build clear visualizations to communicate findings effectively.

## 🧩 Dataset Description
data source : https://www.kaggle.com/datasets/sagnik1511/car-insurance-data/data

The dataset contains customer and vehicle information relevant to car insurance risk.
we have 10,000 records and 12 features

Feature	Description
- CREDIT_SCORE |	Numerical value indicating financial reliability of the policyholder.
- DRIVING_EXPERIENCE|	Categorical variable (Beginner, Experienced, Advanced, Expert) showing years of driving.
- ANNUAL_MILEAGE	|Total miles driven per year (measure of exposure).
- VEHICLE_OWNERSHIP	|Indicates whether the vehicle is owned or financed.
- OUTCOME	|Binary target (0 = No Claim, 1 = Claim).

## 🔍 Exploratory Data Analysis (EDA)

-Key visual and statistical analyses performed:

-Distribution plots for numeric features (e.g., Credit Score, Mileage).

-Bar plots and count plots for categorical variables (e.g., Driving Experience, Vehicle Ownership).

-Correlation analysis to measure strength and direction of feature–target relationships.

-Feature importance extraction using machine learning models.
## 📊 Key Insights
1. Credit Score

Moderate negative correlation with OUTCOME (r = -0.33).

Higher credit scores → lower claim likelihood.

2. Driving Experience

Strong inverse relationship: Beginners have the highest claim rate, Experts the lowest.

Matches expected insurance risk behavior.

3. Annual Mileage

Higher mileage increases claim probability due to greater exposure on the road.

4. Vehicle Ownership

Owned vs. financed vehicles show different risk and claim profiles.

## 💡 Business Interpretation

#### All top features (CREDIT_SCORE, DRIVING_EXPERIENCE, ANNUAL_MILEAGE, and VEHICLE_OWNERSHIP) make strong business sense:

- Drivers with low credit scores or little experience are higher-risk customers.

- More mileage increases exposure to potential accidents.

- Ownership status affects both claim frequency and severity.

- These insights align with standard actuarial reasoning in the insurance industry.

## 🧠 Technologies Used

- language : Python 

- libraries :pandas, numpy ,matplotlib, seaborn ,scikit-learn
  
- Google Colab

  
## 📈 Example Visualizations

#### CREDIT_SCORE vs OUTCOME (Negative correlation)
<img width="555" height="393" alt="credit score" src="https://github.com/user-attachments/assets/a62e540d-5c79-41d8-8ecd-07f2a9f0aca7" />


Studies show that people with higher credit scores tend to file fewer or less severe insurance claims.

This is because credit behavior often correlates with risk behavior — careful financial habits often reflect careful driving habits.

Many insurers legally use credit-based insurance scores as a risk factor (where regulations allow).

✅ Conclusion: credit score is a strong and logical predictor of claim likelihood and risk level.

---
#### DRIVING_EXPERIENCE vs Target Rate (Claim rate decreases with experience)
<img width="567" height="455" alt="car insurance driving ex" src="https://github.com/user-attachments/assets/a9286db9-ac3e-4651-b20c-010b76bc0220" />



✅ Summary:

The plot shows a clear negative relationship between driving experience and the likelihood of a claim. Beginners have the highest risk, while experienced and expert drivers show substantially lower claim rates. This aligns well with expected business logic in auto insurance risk modeling.

---
### Feature importance 
<img width="830" height="547" alt="car insurance dfeature importancepng" src="https://github.com/user-attachments/assets/338f5d1b-bb33-4e78-95b4-862d60f62085" />

we notice from the above plot that features CREDIT_SCORE is the most important one and this makes sense because credit behavior often correlates with risk behavior — careful financial habits often reflect careful driving habits.

the second imortant feature is DRIVING_EXPERIENCE as driving experience directly impacts accident risk

ANNUAL_MILEAGE is the third factor and this makes sense as the more a car is driven, the greater the exposure to potential accidents.

VEHICLE_OWNERSHIP Ownership type can reflect driver responsibility and vehicle condition.

---
## ✅ Final Recommendations
1. Prioritize Risk Assessment Based on Key Predictors:
- Use CREDIT_SCORE, DRIVING_EXPERIENCE, ANNUAL_MILEAGE, and VEHICLE_OWNERSHIP as core features in underwriting and pricing models.
- These variables have strong predictive power and align with established business logic.
- Weight them appropriately in risk scoring or premium calculation formulas.


2. Refine Premium Pricing Strategy
- Implement tiered pricing:
- Low credit score + Beginner drivers + High mileage → higher premiums or stricter underwriting.
- High credit score + Expert drivers + Low mileage → discounts or loyalty incentives.
- Regularly update thresholds using fresh data to ensure fair and data-driven pricing.

3. Encourage Safer Driving Behavior
- Create driver education or incentive programs for beginner and less experienced drivers.
- Offer usage-based insurance (UBI) programs where safe driving habits can reduce premiums.

4. Targeted Marketing & Customer Segmentation:
 Use feature-driven segmentation to design marketing campaigns:
 - Safe, experienced drivers → promote low-cost, reward-based policies.
 -  High-risk groups → emphasize safety tracking apps or telematics-based plans.

5. Monitor and Update Risk Models Regularly
- Periodically retrain and recalibrate predictive models as new claim data becomes available.
- Track feature importance over time to detect shifts in driver behavior or risk patterns.














