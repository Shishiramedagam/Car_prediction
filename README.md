# 🚗 Car Price Prediction using Machine Learning

This project implements a machine learning pipeline for predicting the selling price of used cars based on key features such as year, mileage, fuel type, seller type, transmission, and ownership status. The model is trained using Scikit-learn and evaluated with performance metrics. This project demonstrates preprocessing, encoding, regression modeling, and practical deployment of ML on real-world data.

---

## 📌 Table of Contents

- [Abstract](#abstract)
- [Technologies Used](#technologies-used)
- [Dataset Description](#dataset-description)
- [Workflow](#workflow)
- [Model and Evaluation](#model-and-evaluation)
- [Results](#results)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [License](#license)
- [Author](#author)

---

## 🧾 Abstract

Used car pricing varies significantly depending on brand, model, usage, and condition. This project applies regression-based machine learning techniques to predict car prices accurately. The dataset is processed and modeled using Scikit-learn with techniques such as label encoding, feature selection, and random forest regression. The trained model can be deployed as part of a pricing assistant or a dealer’s recommendation engine.

---

## 🛠 Technologies Used

- Python 3.x  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib / Seaborn  
- Jupyter Notebook

---

## 📊 Dataset Description

- 📁 Source: [Kaggle / open car datasets]
- 📄 Columns:
  - `Car_Name`: Name of the car
  - `Year`: Year of manufacture
  - `Selling_Price`: Price the owner wants
  - `Present_Price`: Price when purchased
  - `Kms_Driven`: Kilometers driven
  - `Fuel_Type`: Petrol, Diesel, or CNG
  - `Seller_Type`: Dealer or Individual
  - `Transmission`: Manual or Automatic
  - `Owner`: Number of previous owners

---

## 🔁 Workflow

1. **Data Cleaning and Exploration**  
2. **Feature Engineering**  
   - Encoding categorical variables  
   - Converting year to car age  
3. **Correlation Analysis and Feature Selection**  
4. **Model Training** using:
   - Random Forest Regressor  
5. **Model Tuning** (via GridSearchCV)  
6. **Model Serialization** (pickle joblib – optional)

---

## 🤖 Model and Evaluation

- **Model Used**: Random Forest Regressor  
- **Train/Test Split**: 80/20  
- **R² Score**: ~0.92 on test set  
- **Error Metrics**:  
  - MAE: Low  
  - RMSE: Acceptable for business usage  

---

## 📈 Results

- Features with highest influence: `Present_Price`, `Kms_Driven`, `Fuel_Type`, `Transmission`  
- The model performs well for most mid-range car predictions  
- Handles categorical-to-numeric conversion smoothly  
- Visualizations show tight residual spread around regression line

---

## 💡 Usage

You can run this notebook to:

1. Understand how ML can be applied to structured data.
2. Explore data transformation, visualization, and correlation.
3. Train and evaluate a regression model.
4. Extend it to include web deployment using Flask/Streamlit (future scope).

---

## 📁 Project Structure

```text
Car_prediction/
├── Car_Predcition01.ipynb     # Main notebook (model building + visualization)
├── car_data.csv               # Dataset file
├── README.md                  # Project documentation
