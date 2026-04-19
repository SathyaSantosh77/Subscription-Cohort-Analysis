# 📊 Subscription Cohort Analysis (Power BI)

## 📌 Project Overview

This project presents a cohort analysis of subscription-based customers using Power BI.
It focuses on understanding **customer retention behavior over time**, tracking how different cohorts of users engage and churn after subscription.

---

## ❓ Business Questions Answered

* How does **customer retention change over time** for different cohorts?
* What percentage of customers **remain active after each month**?
* How does **customer drop-off (churn)** evolve across cohorts?
* Which cohorts show **stronger long-term retention**?

---

## 📊 Data Model

The dataset is structured to support cohort-based analysis:

### 🗂️ Main Table

**Subscription Cohort Analysis Data**

* `customer_id` → Unique customer identifier
* `created_date` → Subscription start date
* `canceled_date` → Subscription end date (if applicable)
* `subscription_cost` → Subscription price
* `subscription_interval` → Billing frequency
* `was_subscription_paid` → Payment status

---

### 📅 Derived Columns

* `Created Date (SOM)` → Cohort grouping (Start of Month)
* `Month List` → Sequential month index
* `Month Span` → Number of months since subscription

---

### 📐 Measures (DAX)

* **Customer Retention %** → Percentage of customers retained over time
* **Customer Retention Volume** → Count of active customers per cohort

---

## 🧠 Analytical Approach

* Grouped customers into cohorts based on **subscription start month**
* Calculated retention using **time-based progression (Month 0 → Month N)**
* Used DAX to dynamically compute:

  * Active customers per cohort
  * Retention percentages
* Visualized results using **cohort heatmaps** for clear trend analysis

---

## 🛠️ Tools & Technologies

* Power BI
* Power Query (Data Transformation)
* DAX (Cohort Calculations & Retention Metrics)

---

## 📈 Dashboard Features

* Cohort heatmap showing **retention % over time**
* Cohort heatmap showing **customer volume decay**
* Time-based cohort comparison across months
* Visual identification of retention trends and drop-offs

---

## 📸 Dashboard Preview

![Cohort Analysis](images/dashboard.png)

---

## 💡 Key Insights

* Retention decreases consistently across cohorts over time
* Majority of customer drop-off occurs within the **first 3–5 months**
* Later cohorts show slightly improved early retention
* Long-term retention stabilizes at a lower percentage across all cohorts

---

## 📢 Conclusion

This project demonstrates the ability to perform cohort analysis, implement retention metrics using DAX, and visualize customer lifecycle behavior.
It highlights how data can be used to understand churn patterns and improve subscription-based business strategies.
