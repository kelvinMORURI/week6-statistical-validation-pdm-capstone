# Capstone Project Proposal: Agricultural Supply Chain & Post-Harvest Loss Mitigation

---

## 👥 Team Members & Roles

| Name | Role |
|------|------|
| **Amos Ndungo** | Data Engineering Lead – pipeline, synthetic data generation, ETL<br>QA & Documentation Lead – testing, UAT notes, deployment readiness |
| **Kevin Nyakundi** | Modeling & ML Lead – hypothesis testing, feature engineering, modeling |
| **Yvonne Wochuna** | Dashboard & Business Analytics Lead – visualization, stakeholder reporting, documentation, storytelling |

---

## 🧩 Problem Statement

Across Sub‑Saharan Africa, smallholder horticultural supply chains experience significant post‑harvest losses, with approximately **30–50% of fresh produce** deteriorating before reaching wholesale markets. These losses reduce farmer incomes, increase food insecurity, and contribute to market price instability.

Current logistics operations rely on static transportation schedules and predetermined delivery routes, which fail because they **do not adapt** to changing environmental conditions such as:
- Ambient temperature & humidity
- Transport delays
- Road congestion
- Fluctuating commodity prices

**Our solution:** Apply geospatial analytics, predictive machine learning, spatial‑temporal feature engineering, and network optimization to estimate produce shelf‑life degradation and dynamically determine optimal transport routes and market destinations.

**Expected impact:**
- Reduce total transportation time by **15–25%**
- Minimize post‑harvest spoilage
- Improve revenue retention for smallholder farmer cooperatives

---

## 🌍 Domain & Context

- **Industry:** Agriculture Technology (AgTech), Supply Chain Analytics, Smart Logistics
- **Geography:** Sub‑Saharan Africa (focus on regional wholesale markets)
- **Commodities:** Perishable horticultural produce (tomatoes, vegetables, fruits, leafy crops)
- **Key drivers:** Prolonged transportation times, poor storage conditions, adverse weather
- **Approach:** Combine agricultural production data, weather observations, logistics telemetry, and market pricing to identify bottlenecks and recommend optimized strategies.

---

## 📊 Dataset Requirements & Schema Overview

The analytical pipeline will integrate multiple publicly available datasets together with simulated logistics data.

| Data Category | Source / Type | Key Variables |
|---------------|---------------|---------------|
| **Primary Agricultural Data** | FAOSTAT | Regional production statistics, historical post‑harvest loss indicators |
| **Climate Data** | CHIRPS, ERA5 | Daily temperature, relative humidity, rainfall intensity |
| **Logistics Data** | Simulated transport telemetry | Vehicle speeds, route distances, stopover durations, vehicle categories |
| **Market Data** | Commodity price databases | Wholesale demand, regional market locations, pricing |

---

## 🎯 Success Metrics

The project will be considered successful if it achieves the following:

- Predict shelf‑life decay using regression models with strong performance (**RMSE, MAE, R²**).
- Reduce transportation duration for perishable shipments by **15–25%**.
- Demonstrate measurable reductions in post‑harvest crop spoilage.
- Increase projected **revenue retention** for participating farmer cooperatives.
- Identify major **transportation bottlenecks** across agricultural corridors.

---

## 📅 Initial Timeline

| Week | Focus | Deliverable |
|------|-------|-------------|
| **7** | Data Collection & Cleaning | Clean agricultural, weather, and logistics datasets |
| **8** | Feature Engineering | Generate spatial‑temporal variables, heat exposure indicators, route friction metrics |
| **9** | Machine Learning Modeling | Train Random Forest, XGBoost, and regression models |
| **10** | Route Optimization | Develop graph‑based routing using NetworkX and Linear Programming |
| **11** | Dashboard Development | Build interactive Streamlit dashboard and visual analytics |
| **12** | Final Deployment | Complete documentation, presentation, and final demonstration |

---

## 🔍 Key Research Questions

1. **Spoilage Prediction**  
   How accurately can transportation duration, road quality, temperature, and humidity predict post‑harvest spoilage?

2. **Supply Chain Bottlenecks**  
   Which transportation corridors contribute most significantly to delays and crop deterioration?

3. **Economic Impact**  
   How much additional revenue can farmer cooperatives retain through optimized routing that reduces transportation time by 15–25%?

---

## 🎯 Core Project Objectives

- **Exploratory Data Analysis**  
  Analyze relationships between transportation variables, climate conditions, storage methods, and historical spoilage rates.

- **Predictive Modeling**  
  Develop machine learning models capable of estimating produce shelf‑life degradation under varying transportation and environmental conditions.

- **Geospatial Optimization**  
  Design a graph‑based routing system that recommends optimal market destinations based on transportation efficiency, commodity demand, and pricing.

- **Decision Support Dashboard**  
  Build an interactive dashboard that enables logistics managers to monitor transportation risks, visualize spoilage hotspots, and recommend optimal dispatch routes.

---

## 🛠️ Technical Approach & Methodology

| Phase | Analytical Focus | Methods & Tools | Expected Outputs |
|-------|------------------|-----------------|------------------|
| **Data Ingestion** | Data cleaning, spatial matching, timestamp alignment | Pandas, NumPy, GeoPandas | Cleaned master tabular & GIS dataset |
| **Feature Engineering** | Calculating thermal heat exposure during transit, route friction indices | Spatial Join, Haversine metrics, Feature Scaling | Engineered transit risk indicators |
| **Modeling** | Spoilage rate prediction & demand forecasting | Scikit‑learn (Random Forest, XGBoost), Prophet | Evaluated ML models (RMSE, R², MAE) |
| **Optimization** | Shortest path & market price yield maximization | NetworkX, Linear Programming (PuLP) | Dynamic routing decision algorithm |
| **Dashboard Visualization** | Interactive decision‑support system | Streamlit, Plotly | Real‑time monitoring and routing interface |

---

## 📦 Expected Capstone Deliverables

1. **Comprehensive Data Pipeline**  
   A fully documented Python pipeline for data ingestion, preprocessing, feature engineering, and predictive modeling.

2. **Analytical Report**  
   A comprehensive evaluation of post‑harvest loss drivers, together with policy recommendations and logistics optimization strategies.

3. **Interactive Dashboard** (Streamlit)  
   Visualizing:
   - Spoilage hotspots
   - Transportation bottlenecks
   - Weather conditions
   - Market price opportunities
   - Recommended transport routes

---

## 📎 Conclusion

This capstone project bridges **data science**, **geospatial analysis**, and **supply chain logistics** to tackle one of the most pressing challenges in African agriculture. By leveraging predictive modeling and optimization, we aim to turn data into actionable insights that reduce waste, increase farmer incomes, and build more resilient food systems.

---

*Prepared by Team KPC · Inuka Fellowship (Power Learn Project)*
