# Telco Customer Churn: A Strategic Growth & Retention Analysis

## 📌 Project Overview
This analysis identifies the primary drivers of customer attrition to **protect revenue and optimize Customer Lifetime Value (LTV)**. By transforming raw data into actionable insights, this project serves as a blueprint for data-driven retention strategies.

The goal was to provide the Growth team with two high-leverage answers: 
1. **Segment Prioritization:** Which users represent the highest churn risk and "lost revenue" potential?
2. **Product Stickiness:** Which service "anchors" can be bundled to increase retention and ROI?

## 📊 The Dataset
The dataset used for this analysis is the **Telco Customer Churn** dataset from Kaggle.
* **Source:** [Kaggle - Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
* **Scope:** 7,043 customers including demographic info, account details (tenure, contract, charges), and services.

## 🔍 Growth Insights & Key Findings

### 1. The "Contract Gap" & LTV Risk
Contract type is the single greatest predictor of customer stability. 
* **Month-to-Month:** ~43% churn rate.
* **Two Year:** 2.8% churn rate.
* **Growth Takeaway:** Moving a customer from month-to-month to a contract isn't just a "billing change"—it **increases their expected LTV by over 15x.**

<img width="934" height="573" alt="image" src="https://github.com/user-attachments/assets/1525f231-643c-41e5-a62f-b1890b3fe0f4" />

### 2. The Critical "Onboarding Window"
Using a **Seaborn Regression Plot**, I identified that churn risk is highest in the first few months of the customer lifecycle.
* **Growth Takeaway:** Retention is won or lost in the first 90 days. This identifies a "Critical Window" for **automated win-back and engagement campaigns.**

<img width="1170" height="692" alt="image" src="https://github.com/user-attachments/assets/4a30634d-5d9c-438e-80e0-5c340e23277b" />

### 3. The $80 "Value Gap"
I mapped churn probability against monthly charges using a **KDE (Kernel Density Estimate) Plot**.
* **Finding:** Churn spikes at the **$80/month mark**, particularly for Fiber Optic users.
* **Growth Takeaway:** This suggests a "Price-to-Value" disconnect. We are acquiring customers at a premium price point but failing to provide the "stickiness" required to keep them.

<img width="1170" height="692" alt="image" src="https://github.com/user-attachments/assets/9af4f87f-3f0d-4a7d-b80a-f95b602ef70f" />

### 4. The "Security Anchor" (Bundling Strategy)
The most actionable discovery: **Online Security** acts as a powerful retention lever for premium Fiber customers.
* **Finding:** Adding Online Security **cuts churn in half (50% down to 25%)** for the highest-spending segment.
* **Growth Takeaway:** Bundling security services is a high-margin way to "lock in" users without needing to lower the base price.

<img width="1171" height="691" alt="image" src="https://github.com/user-attachments/assets/7d852b90-4f57-44d8-99fa-4505745c4631" />

## 🛠️ Technical Skills Demonstrated
* **Predictive Modeling Prep:** Engineered `Churn_Binary` features to allow for advanced statistical aggregation and trend-line analysis.
* **Statistical Visualization:** Leveraged **Seaborn** to create Regression Plots and KDE Plots to visualize customer behavior density
