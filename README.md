# Health_Care_Premium_Prediction_ML
Project on predicting health premium score using Machine Learning based on the necessary users health related inputs or data's 


## 🔍 Exploratory Data Analysis (EDA)

To better understand the dataset and identify patterns affecting health insurance premiums, extensive exploratory data analysis was performed using Seaborn and Matplotlib.

### EDA Techniques Used

* Univariate Analysis
* Bivariate Analysis
* Correlation Analysis
* Heatmaps
* Bar Plots
* Distribution Analysis

### Outlier Handling

* Detected and handled outliers using the Interquartile Range (IQR) method.
* Reduced the impact of extreme values on model performance.

---

## ⚙️ Feature Engineering

Several feature engineering techniques were applied to improve prediction performance:

### Medical Risk Encoding

Medical history information was transformed into risk-based numerical representations by assigning disease risk scores.

### Feature Scaling

* Applied Min-Max Scaling to normalize numerical features.
* Improved model stability and comparability across variables.

### Multicollinearity Check

Variance Inflation Factor (VIF) analysis was performed to identify highly correlated features.

**Criteria Used:**

* VIF < 10 → Acceptable
* VIF > 10 → Investigated and handled appropriately

---

## 🤖 Model Development

Instead of using a single model for all customers, a segmented modeling approach was implemented.

### Young Age Group Model (18–25 Years)

* Linear Regression was used.
* Initially produced lower performance.
* After incorporating additional training data and feature improvements, prediction accuracy improved significantly.

### Adult Age Group Model (Above 25 Years)

* XGBoost Regressor was used.
* Demonstrated superior performance for more complex premium prediction patterns.

### Model Segmentation Strategy

Different age groups exhibit different premium trends. Therefore:

| Age Group      | Model Used        |
| -------------- | ----------------- |
| 18–25 Years    | Linear Regression |
| Above 25 Years | XGBoost Regressor |

This hybrid approach improved overall prediction quality by leveraging the strengths of each algorithm.

---

## 🔧 Hyperparameter Tuning

To optimize model performance:

### Ridge Regression

* Used as a regularized baseline model.

### XGBoost Optimization

* Applied RandomizedSearchCV for hyperparameter tuning.
* Evaluated multiple parameter combinations efficiently.
* Selected the best-performing configuration based on validation performance.

---

## 📈 Model Evaluation

Models were evaluated using regression metrics such as:

* R² Score
* RMSE (Root Mean Squared Error)

Performance was assessed separately for each age segment to ensure robust predictions across customer groups.

---

## 🌐 Deployment

A user-friendly web application was developed using Streamlit.

### Features

* Interactive Input Form
* Real-Time Premium Prediction
* Segment-Based Model Selection
* Fast Response Time
* Clean and Responsive Interface

The application was successfully deployed on Streamlit Cloud, enabling users to access premium predictions directly through a web browser.

---

## 💡 Key Project Highlights

✅ End-to-End Machine Learning Pipeline

✅ Outlier Detection using IQR

✅ Comprehensive EDA with Seaborn

✅ Heatmap-Based Correlation Analysis

✅ Disease Risk Score Encoding

✅ Min-Max Feature Scaling

✅ Multicollinearity Analysis using VIF

✅ Hyperparameter Tuning using RandomizedSearchCV

✅ Ridge Regression and XGBoost Modeling

✅ Age-Based Model Segmentation

✅ Streamlit Web Application Development

✅ Cloud Deployment using Streamlit Cloud

## 📷 Screenshots:

### Home Page

<img width="997" height="750" alt="Screenshot 2026-06-10 141353" src="https://github.com/user-attachments/assets/7f32de95-52ca-4ad7-baa4-c47c4ac9e46d" />

### Prediction Result

<img width="963" height="757" alt="Screenshot 2026-06-10 141557" src="https://github.com/user-attachments/assets/274dfd13-1b5b-40c3-9242-012382f8addc" />

