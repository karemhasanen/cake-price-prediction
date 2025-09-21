# 🎂 Cake Price Prediction using Machine Learning

This project showcases a complete machine learning workflow to predict the price of cakes. Using a dataset that includes features like ingredient cost, size, and design complexity, a Random Forest Regressor is trained to provide accurate price estimates.

---

## 📌 Project Highlights

- **High Accuracy**: Achieves a low Mean Absolute Error (MAE), with predictions being off by only ~\$15 on average.  
- **Full ML Pipeline**: Covers data cleaning, exploratory data analysis, feature engineering, and model evaluation.  
- **Ethical Consideration**: Proactively removes the `Gender` feature to prevent potential bias in pricing.  
- **Technology**: Built with Python, Scikit-learn, and Pandas.  

---

## 📋 Table of Contents

- [Project Objective](#project-objective)  
- [Dataset](#dataset)  
- [Methodology](#methodology)  
- [Results & Evaluation](#results--evaluation)  
- [How to Run This Project](#how-to-run-this-project)  

---

## Project Objective

The primary goal is to build a robust regression model that can accurately predict the price of a cake based on its various attributes. This serves as a practical application of machine learning for a real-world business problem.

---

## Dataset

The dataset used for this project contains 4,000 entries with the following features:

- **Sold_On**: The day of the week the cake was sold.  
- **Size**: The size of the cake (small, medium, large).  
- **Ingredients_Cost**: The cost of the raw materials.  
- **Design_Complexity**: Whether the design is simple or complex.  
- **Time_Taken**: The time in hours required to bake and decorate the cake.  
- **Amount**: The quantity of similar cakes in the same order.  
- **Price**: The final price of the cake (the target variable).  

---

## Methodology

The project follows a structured machine learning workflow:

1. **Data Cleaning & Preprocessing**  
   - Checked for missing values (none found).  
   - Removed the `Gender` column (not correlated with price + potential bias).  

2. **Exploratory Data Analysis (EDA)**  
   - Strong positive correlation (**0.91**) between `Ingredients_Cost` and `Price`.  
   - `Time_Taken` also strongly correlated with `Price`.  
   - Prices clearly increase with `Size` and `Design_Complexity`.  

3. **Feature Engineering**  
   - **Ordinal Encoding**: `Size` mapped (`small=0`, `medium=1`, `large=2`).  
   - **One-Hot Encoding**: Nominal features (`Sold_On`, `Design_Complexity`).  

4. **Model Training**  
   - Chosen model: **Random Forest Regressor** (handles non-linear data well).  
   - Training on 80% of dataset, testing on 20%.  

---

## Results & Evaluation

The model's performance on the test set:

| Metric                      | Value       |
| --------------------------- | ----------- |
| **Mean Absolute Error (MAE)** | **~\$14.88** |
| **Root Mean Squared Error (RMSE)** | **~\$18.84** |

➡️ On average, predictions are only **\$14.88** off from actual prices, which is highly accurate given the dataset’s price range.  

---

   git clone https://github.com/your-username/cake-price-prediction.git
   cd cake-price-prediction
