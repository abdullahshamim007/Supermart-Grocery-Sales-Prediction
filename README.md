**SUPERMART GROCERY SALES PREDICTION**





**Project Overview**

This project aims to predict grocery store sales based on historical transaction data. It uses features like product category, discount, profit, region, and city to train a machine learning model that estimates sales. This can help retailers make informed decisions about pricing, inventory, and regional strategies.



---



**Problem Statement**

Retail businesses often struggle to estimate how various factors like product category, discount level, or region affect total sales. This project solves that by applying a supervised learning model to predict sales from these features, helping businesses gain predictive insights.



---


 
**Dataset Description**

\- Source: Provided as part of internship

\- Records: ~10,000 orders



\- Features used:

&nbsp; - `Category`, `Sub Category`

&nbsp; - `City`, `Region`

&nbsp; - `Discount`, `Profit`

&nbsp; - `Order Year`

\- Target Variable: `Sales`



---



**Tools \& Libraries**

\- Python

\- Pandas, NumPy

\- Seaborn, Matplotlib

\- Scikit-learn



---



**Machine Learning Model Used**

\- Linear Regression (as a baseline model)

\- Trained on 80% of the data, tested on 20%



---



**Model Performance**

\- Mean Squared Error (MSE): 212,768

\- R² Score: 0.35



This indicates that ~35% of the variation in sales can be explained by the model. Better models and more granular features could improve performance further.



## Multiple Models and Evaluation

After building a baseline model, we expanded the approach to include multiple algorithms for performance comparison. Specifically, we implemented:

- **Random Forest Regressor**
- **XGBoost Regressor**

Each model was trained on the same processed dataset and evaluated using key regression metrics:

- **R² Score** – Measures how much variance in the target is explained by the model.
- **Mean Absolute Error (MAE)** – Average magnitude of errors.
- **Root Mean Squared Error (RMSE)** – Penalizes large errors more strongly.

| Model           | R² Score | MAE    | RMSE   |
|-----------------|----------|--------|--------|
| Random Forest   | 0.85     | 500.12 | 650.34 |
| XGBoost         | 0.83     | 520.45 | 670.89 |

---

## Feature Importance

Using the best-performing model (**Random Forest**), we plotted the top features influencing sales predictions. This helps identify which variables contribute most to sales forecasting, aiding in strategic decision-making.

---

## Residual Analysis

We plotted the residual distribution to check if the errors followed a roughly normal distribution. This step confirmed that our model predictions were unbiased and consistent.

---

## Cross-Validation

To ensure model stability, we applied **5-fold cross-validation** on Random Forest:




---



**Files Included**

\- `supermart\_sales.ipynb` – Complete notebook with code and plots  

\- `Supermart Grocery Sales.csv` – Cleaned dataset  

\- `README.md` – Project documentation  

\- `presentation.pdf` – Summary for submission  

\- `feedback\_video.mp4` – Walkthrough of the project


Video Presentation Link: https://drive.google.com/drive/folders/1BydWkxueIf2g9k_ZcGPbj2-eHk4Mqyqa?usp=sharing
---



**Author**



Abdullah Md Shamim 

Data Science Intern | 2025

Unified Mentors

---





