# 🚗 Used Car Price Prediction – India Case Study

## 🎯 Objective

To perform exploratory data analysis on a dataset of used cars in India in order to identify the factors that affect the price of a used car, and build a predictive model to estimate prices for unseen data.

---

## 📌 Problem Statement

A leading used-car seller in India is aiming to enhance its ability to predict the **on-spot price estimate** of used cars. With historical data on hand, the company seeks to identify key pricing factors and apply regression-based analytics to expedite the evaluation of unsold cars.

---

## 📊 Dataset Summary

- **Duration Covered**: 1998 to 2019 (22 years)
- **Training Data**: `Sample data-used cars India.csv`
  - Records: 6019 rows
  - Features: 13 columns
- **Test Data**: `test-data.csv`
  - Records: 1234 rows

---

## 🧩 Task Breakdown

### 1. 🔄 Data Preprocessing

- Renamed columns and standardized units where applicable.
- Handled missing values appropriately.
- Categorical variables identified and encoded using **dummy encoding**.
- Continuous variables identified and scaled if necessary.
- Final dataset prepared for regression modeling.

### 2. 📈 Exploratory Data Analysis (EDA)

- Identified:
  - **Categorical Variables**: Car Name, Fuel Type, Transmission, Owner Type, Location, etc.
  - **Continuous Variables**: Year, Kilometres Driven, Engine (CC), Power (BHP), Mileage, etc.
- Created:
  - Histograms and box plots to explore distributions
  - Pivot tables and bar charts to analyze average price by brand
  - Scatter plots for variable interaction (e.g., Kilometers vs Price)
- Found that:
  - **Kilometers Driven** is **negatively correlated** with price.
  - **Maruti, Hyundai, and Honda** are the most frequently sold brands.
  - Categorical variables such as **Transmission** and **Fuel Type** show a clear impact on price.

### 3. 🔍 Correlation & Feature Selection

- Correlation analysis revealed key factors affecting price.
- Selected variables with **p-value < 0.05** for inclusion in the regression model.
- Notable variables: `Car Name`, `Location`, `Year`, `Kilometres Driven`, `Transmission`, `Engine`, `Seats`.

### 4. 🧮 Model Building

- Built a **Linear Regression Model** on the training data.
- Achieved:
  - **Training Data R²**: 0.73
  - **Training MSE**: 37.3
- Applied model on test data and obtained:
  - **Test Data R²**: 1.0 *(Note: High accuracy may imply overfitting or low variance in test set)*

---

## 🤖 Model Application

- Predictive model built can estimate the **price of a used car** based on features such as age, kilometers driven, engine capacity, location, and more.
- Model applied on the test dataset to estimate prices for 1234 unseen car entries.

---

## ✅ Conclusion

- Successfully identified key pricing factors using EDA and regression analysis.
- Model performed reliably, especially on structured test data.
- Demonstrated that features like **car brand**, **location**, **engine size**, and **transmission type** significantly affect used car prices.

---

## 🌟 Benefits & Use Cases

- Enables **faster, data-driven price estimation** for used car resellers.
- Offers **buyers and sellers** insights into the primary factors that affect car prices.
- Supports the development of **automated pricing tools** to scale used-car businesses efficiently.

---

## 🛠️ Tools & Technologies Used

- **Language**: Python
- **Libraries**: Pandas, NumPy, Seaborn, Matplotlib, Scikit-learn
- **Environment**: Jupyter Notebook / Google Colab

---

## 📬 Contact

For more information or queries, feel free to reach out!

Happy Analyzing! 🚘📊
