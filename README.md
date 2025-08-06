## 🧪 **Predictive Modeling of Access to Improved Drinking Water in India**

### 🔍 Overview

This project focuses on developing a machine learning model to predict the percentage of population with access to improved sources of drinking water in India. Using government survey data from the **78th Round of the NSSO Multiple Indicator Survey**, the model identifies regional and demographic disparities in access to water. The goal is to generate actionable insights that support **evidence-based policy decisions** aligned with **Sustainable Development Goal 6 (Clean Water and Sanitation)**.

---

### 📁 Dataset

The dataset used in this project is publicly available from the **National Sample Survey Office (NSSO)**, Government of India. The CSV file `nss Items data.csv` contains records with the following columns:

* `State`
* `Age Group`
* `Sector` (Rural / Urban / All)
* `Gender`
* `Indicator` (e.g., Access to drinking water, use of clean cooking fuel)
* `Value` (percentage of population related to the indicator)

---

### 🧠 Problem Statement

Despite ongoing efforts, many regions in India — especially rural and underdeveloped areas — still face significant challenges in accessing clean and safe drinking water. This project aims to address that gap by using **machine learning** to:

* Predict the `Value` (percentage) based on demographic inputs
* Discover patterns and disparities in water access across regions

---

### ⚙️ Tools & Technologies

* **IBM Cloud** – Platform for development and deployment
* **IBM Watsonx.ai Studio** – Used for model training and AutoAI
* **AutoAI** – IBM’s automated machine learning engine
* **Model Deployed As:** Online REST API using Watson Machine Learning
* **Algorithm Used:** XGBoost Regressor (selected by AutoAI)

---

### 📊 Model Pipeline

1. Dataset uploaded to Watsonx.ai Studio
2. Target column set as `Value`
3. AutoAI handled:

   * Data preprocessing
   * Feature transformation
   * Model selection
4. Best pipeline: **XGB Regressor**
5. Model deployed online with API access enabled

---

### 📈 Results

* **R² Score:** 0.87
* **MAE (Mean Absolute Error):** \~2.5%
* Sample predictions showed strong alignment with real survey percentages

---

### 🚀 Future Scope

* Add features like income, education, sanitation level
* Visualize results using maps or dashboards
* Scale predictions to district or village level for granular insights
* Integrate with public-facing dashboards for NGOs and policymakers

---

### 📄 References

* [NSSO 78th Round - MIS Survey](https://mospi.gov.in)
* [IBM Watsonx.ai Documentation](https://dataplatform.cloud.ibm.com)
* [UN SDG 6: Clean Water & Sanitation](https://sdgs.un.org/goals/goal6)
* [XGBoost Documentation](https://xgboost.readthedocs.io)

