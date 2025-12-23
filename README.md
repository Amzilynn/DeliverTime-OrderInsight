# DeliverTime & OrderInsight  

---

## Project Overview

This project tackles two core business challenges in the food delivery industry:

1. **Supervised Learning**: Predict accurate delivery times using regression models to improve customer experience.
2. **Unsupervised Learning**: Cluster customer orders to uncover consumption patterns and support targeted marketing strategies.

The notebook follows a structured CRISP-DM approach, covering:
- Business Understanding
- Data Understanding (Exploratory Data Analysis)
- Data Preparation
- Modeling & Evaluation
- Insights & Recommendations

---

##  Objectives

###  Supervised Learning (Regression)
- **Business Objectif**: Improve customer satisfaction by providing reliable delivery time estimates.
- **Data Science Objectif**: Predict delivery duration (in minutes) using features like:
  - Order size
  - Restaurant category
  - Time of day
  - Delivery partner availability
  - Weather & traffic conditions
- **Models Used**: Linear Regression (initial suggestion)
- **Evaluation Metrics**: RMSE, MAE, R²

### ✅ Unsupervised Learning (Clustering)
-  **Business Objectif**: Understand customer consumption habits to optimize marketing and operations.
- **Data Science Objectif**: Cluster orders based on:
  - Items ordered
  - Order value
  - Time of day
  - Category preferences
- **Model Used**: K-Means Clustering
- **Evaluation Metrics**: Silhouette Score, Davies-Bouldin Index

---

## Dataset

- **File**: `datadelevry.csv`
- **Size**: ~172,941 rows, 14 columns
- **Features Include**:
  - `market_id`, `created_at`, `actual_delivery_time`
  - `store_id`, `store_primary_category`
  - `total_items`, `subtotal`, `num_distinct_items`
  - `min_item_price`, `max_item_price`
  - `total_onshift_partners`, `total_busy_partners`, `total_outstanding_orders`

---

## Tech Stack

- **Language**: Python
- **Libraries**:
  - `pandas`, `numpy`
  - `matplotlib`, `seaborn`
  - `scikit-learn` (for modeling)
  - `pickle` (for model serialization)
- **Environment**: Google Colab / Jupyter Notebook

---

## Key Steps

1. **Data Loading & Inspection**
2. **Missing Values Analysis**
3. **EDA & Visualization** (Boxplots, distributions, correlations)
4. **Feature Engineering**
5. **Model Training & Evaluation**
6. **Clustering Analysis & Interpretation**
7. **Model Deployment** (via pickled models: `kmeans_model.pkl`, `scaler.pkl`, `feature_columns.pkl`)

---

## How to Run

1. Upload the dataset and notebook to Google Colab or a local Jupyter environment.
2. Mount Google Drive (if using Colab) and set the correct file paths.
3. Run cells sequentially to:
   - Load and explore data
   - Train regression and clustering models
   - Evaluate performance
   - Save models for deployment

---

##  Results & Insights

- Delivery time predictions help in:
  - Setting accurate customer expectations
  - Optimizing delivery routes
  - Reducing customer complaints
- Order clustering reveals segments such as:
  - High-value evening orders
  - Quick lunchtime orders
  - Price-sensitive customers

---

##  Stakeholders

- **Logistics Managers** → Optimize delivery routes
- **Customer Service Teams** → Manage customer expectations
- **Marketing Department** → Design targeted campaigns
- **Sales Teams** → Personalize offers based on order habits

---

##  Success Criteria

- Measurable increase in Customer Satisfaction Score 
- Actionable insights leading to optimized logistics and marketing strategies
- Clear, interpretable clusters that guide business decisions
