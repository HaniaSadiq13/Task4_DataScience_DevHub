# Task 4: Predicting Insurance Claim Amounts

## 🎯 Objective
Estimate **medical insurance claim amounts** based on personal attributes such as age, BMI, and smoking status using **Linear Regression**.

## 📁 Dataset
- **Name**: Medical Cost Personal Dataset  
- **Source**: Kaggle (or `insurance.csv`)  
- **Target Variable**: `charges` (total medical insurance cost)

## 🛠️ Libraries Used
- `pandas` and `numpy` – for data manipulation  
- `matplotlib.pyplot` and `seaborn` – for visualization  
- `scikit-learn` – for modeling and evaluation  

## 🔍 Steps Performed

### 1. Load and Inspect Dataset
- Loaded using `pandas.read_csv()`
- Displayed shape, columns, and first few rows with `.shape`, `.columns`, and `.head()`

### 2. Encode Categorical Features
- Encoded `sex`, `smoker`, and `region` using `LabelEncoder`

### 3. Visualize Feature Impact
- **Scatter plots**:
  - Age vs Charges
  - BMI vs Charges
- **Box plot**:
  - Smoker vs Charges
- Observed that **smoking** and **BMI** significantly affect charges

### 4. Train Linear Regression Model
- Defined `X` (features) and `y` (target: `charges`)
- Split the data using `train_test_split`
- Trained a **Linear Regression** model

### 5. Evaluate Model Performance
- Evaluated using:
  - **Mean Absolute Error (MAE)**
  - **Root Mean Squared Error (RMSE)**

## 📊 Results

| Metric | Value (approx) |
|--------|----------------|
| MAE    | ~4200          |
| RMSE   | ~6100          |

> *Performance depends on train-test split and dataset variations.*

## 📌 Key Skills Demonstrated
- ✅ Regression modeling with Linear Regression  
- ✅ Data encoding for categorical features  
- ✅ Feature impact visualization using scatter and box plots  
- ✅ Model evaluation using MAE and RMSE

## 🧠 Potential Improvements
- Use **polynomial regression** or **regularized models** (Ridge, Lasso)  
- Perform **feature selection** and **outlier handling**  
- Apply **one-hot encoding** for categorical data for better results
