# -FUTURE_ML_01
# Sales & Demand Forecasting System

This project is a **Sales and Demand Forecasting System** developed as part of the **Future Interns** Machine Learning Internship (Task 1). The system analyzes historical sales data from the Global Superstore dataset and predicts future sales values using an advanced Machine Learning Regressor.

---

 🚀 Project Overview
The objective of this project is to build a predictive model that can accurately forecast future product sales based on various business parameters such as product category, sub-category, geographic region, quantity ordered, and expected profit margins.

---

🛠️ Tech Stack & Libraries Used
* **Language:** Python 3
* **Environment:** Jupyter Notebook / Google Colab
* **Data Manipulation:** Pandas, NumPy
* **Machine Learning:** Scikit-Learn (sklearn)
  * `LabelEncoder` (for data preprocessing)
  * `train_test_split` (for dataset splitting)
  * `RandomForestRegressor` (Core ML algorithm)
  * `mean_absolute_error`, `r2_score` (Model evaluation metrics)

---

 📈 Key Steps Implemented

1. Data Loading & Inspection
* Successfully loaded the historical dataset (`Global Superstore.csv`) into a Pandas DataFrame.
* Selected the core features critical for predicting sales: `Category`, `Sub-Category`, `Region`, `Quantity`, `Profit`, and `Year`.

 2. Data Cleaning & Preprocessing
* Checked for and validated that there were **0 missing (null) values** in the selected subset.
* Converted text-based categorical columns (`Category`, `Sub-Category`, `Region`) into numerical formats using **Label Encoding** so the Machine Learning model could interpret them.

3. Model Training & Splitting
* Separated the data into Features ($X$) and Target variable ($y$ - Sales).
* Split the dataset into **80% Training data** (to teach the model) and **20% Testing data** (to validate accuracy).
* Implemented and trained a **Random Forest Regressor** model with 100 decision trees.

 4. Live Forecasting
 Integrated an interactive mechanism that takes custom inputs (e.g., Category, Sub-Category, Region, Quantity, Expected Profit, and Year) and outputs a real-time forecasted sales value.

---

 📊 Model Evaluation Results

After training and testing the model against unseen historical data, the evaluation metrics achieved are:

Mean Absolute Error (MAE):** 97.47  *(Indicates high precision in individual price forecasting)*
R2 Score (Model Accuracy):** **63.62%** ---

📂 How to Run the Project
1. Clone this repository or download the files.
2. Place the `Global Superstore.csv` dataset in the same folder as the `data sales.ipynb` file.
3. Open Jupyter Notebook, run all cells sequentially from top to bottom, and enter your inputs when prompted for live forecasting!
