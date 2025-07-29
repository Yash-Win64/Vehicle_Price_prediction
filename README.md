# Vehicle_Price_prediction
This project builds a machine learning model that predicts the **price of a used vehicle** based on its specifications such as make, model, mileage, fuel type, transmission, and more.

---

## 📌 Objective

To help users estimate the resale value of vehicles using machine learning techniques on structured vehicle specification data.

---

## 📂 Dataset

The dataset includes information on vehicle specifications and their corresponding prices.

**Features include:**
- `name`: Full vehicle name
- `make`, `model`, `trim`
- `year`, `mileage`, `cylinders`, `fuel`, `transmission`, `body`, `drivetrain`
- `exterior_color`, `interior_color`
- `price`: Target variable (USD)

---

## ⚙️ Project Workflow

1. **Data Cleaning**  
   - Removed duplicates, null values, and invalid entries (e.g., price = 0)
2. **Feature Engineering**  
   - Extracted `vehicle_age` from `year`
   - Encoded categorical variables (OneHotEncoding)
3. **EDA (Exploratory Data Analysis)**  
   - Visualized relationships between price and features
4. **Model Training**  
   - Trained a `RandomForestRegressor` using pipeline
   - Evaluated using RMSE and R² score
5. **Model Saving**  
   - Saved using `joblib` for later prediction

---

## 🧠 ML Model

- Model: `RandomForestRegressor`
- Evaluation:
  - **R² Score**: ~0.91
---

## 📊 Visualization (EDA Highlights)

- Price distribution histogram
- Fuel type vs. price boxplot
