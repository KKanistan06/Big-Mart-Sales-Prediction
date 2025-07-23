# Big Mart Sales Prediction

<img src="https://raw.githubusercontent.com/kaniskanay/sample-assets/main/bigmart_sales_banner.png" width="1000" height="500">

![Python Version](https://img.shields.io/badge/Python-3-blue) 
![GitHub Pull Requests](https://img.shields.io/github/issues-pr/shreyapatil1199/Big_Mart_Sales_Prediction) 
![GitHub Stars](https://img.shields.io/github/stars/shreyapatil1199/Big_Mart_Sales_Prediction)

This project predicts product sales for Big Mart outlets using machine learning techniques. The goal is to build accurate predictive models that help in decision-making related to inventory, pricing, and store management.

---

## 📚 Table of Contents
- [Project Overview](#project-overview)
- [Dataset Description](#dataset-description)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Model Building](#model-building)
- [Evaluation Metrics](#evaluation-metrics)
- [Insights & Recommendations](#insights--recommendations)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Installation](#installation)

---

## 📝 Project Overview

Big Mart operates retail stores across various cities. The aim of this project is to forecast the **Item Outlet Sales** using historical data. This will aid Big Mart in:

- Optimizing inventory across stores
- Adjusting pricing and promotional strategies
- Improving profitability through data-driven decisions

---

## 📦 Dataset Description

The dataset includes both product and store-level attributes.

| Column | Description |
|--------|-------------|
| `Item_Identifier` | Unique ID for each product |
| `Item_Weight` | Weight of the product |
| `Item_Fat_Content` | Fat level of the item (`Low Fat`, `Regular`) |
| `Item_Visibility` | Visibility in store (%) |
| `Item_Type` | Product category (`Snacks`, `Fruits`, etc.) |
| `Item_MRP` | Maximum Retail Price |
| `Outlet_Identifier` | Store ID |
| `Outlet_Establishment_Year` | Store establishment year |
| `Outlet_Size` | Size of store (`Small`, `Medium`, `High`) |
| `Outlet_Location_Type` | Urban/rural/tier |
| `Outlet_Type` | Type of outlet (`Supermarket Type1`, etc.) |
| `Item_Outlet_Sales` | **Target variable** — sales of the item at the outlet |

---

## 📊 Exploratory Data Analysis (EDA)

EDA was performed to understand the relationships between features and identify patterns. Techniques used:

- Handling missing values (`Item_Weight`, `Outlet_Size`)
- Encoding categorical variables
- Distribution analysis of target variable
- Correlation heatmaps
- Box plots for outliers

---

## 🤖 Model Building

Machine learning models used for regression:

- **Linear Regression**
- **Decision Tree Regressor**
- **Random Forest Regressor**
- **XGBoost Regressor**

Techniques:

- Train-test split (70-30)
- GridSearchCV for hyperparameter tuning
- StandardScaler for normalization

---

## 🧪 Evaluation Metrics

The models were evaluated using:

- **Root Mean Squared Error (RMSE)**
- **R² Score**
- **Mean Absolute Error (MAE)**

Best performance was achieved using Random Forest and XGBoost.

---

## 💡 Insights & Recommendations

- **Item MRP** is the most important feature influencing sales.
- **Outlet Type** and **Item Type** also play significant roles.
- Smaller outlets show lower average sales — promotions can help boost them.
- Improving item visibility in-store positively correlates with higher sales.

---

## 🚀 Usage

To run the project locally:

```bash
git clone https://github.com/KKanistan06/Big_Mart_Sales_Prediction.git
cd Big_Mart_Sales_Prediction
jupyter notebook
