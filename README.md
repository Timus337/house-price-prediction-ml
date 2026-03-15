# 🏠 House Price Prediction using Machine Learning

## 📌 Project Overview

This project builds a **Machine Learning model to predict house prices** based on various housing features such as number of bedrooms, bathrooms, living area, floors, and construction year.

The goal of the project is to demonstrate the **end-to-end machine learning workflow**, including:

* Data loading and preprocessing
* Data exploration and visualization
* Feature selection
* Model training
* Model evaluation

The model is trained using **Linear Regression** and evaluated using standard regression metrics.

---

# 📊 Dataset

The dataset used in this project is the **King County House Sales Dataset**, which contains house sale prices in King County, USA.

### Selected Features

| Feature      | Description                    |
| ------------ | ------------------------------ |
| bedrooms     | Number of bedrooms             |
| bathrooms    | Number of bathrooms            |
| sqft_living  | Living area size (square feet) |
| floors       | Number of floors               |
| yr_built     | Year the house was built       |
| yr_renovated | Year the house was renovated   |

### Target Variable

| Variable | Description      |
| -------- | ---------------- |
| price    | House sale price |

---

# ⚙️ Machine Learning Pipeline

The project follows a structured ML workflow:

### 1️⃣ Data Loading

* Dataset imported using **Pandas**

### 2️⃣ Data Exploration

* Statistical summary
* Missing value checks
* Feature inspection

### 3️⃣ Data Visualization

Relationships between features and price were explored using scatter plots and visualizations.

Examples:

* `sqft_living` vs `price`
* `floors` vs `price`
* `yr_renovated` vs `price`

### 4️⃣ Feature Selection

Relevant numerical features were selected for training the model.

### 5️⃣ Train/Test Split

The dataset was split using:

* **80% Training Data**
* **20% Testing Data**

This ensures the model can generalize to unseen data.

### 6️⃣ Model Training

A **Linear Regression model** from `scikit-learn` was trained using the selected features.

### 7️⃣ Model Evaluation

The model performance was evaluated using:

* **Mean Squared Error (MSE)**
* **R² Score**

Example result:

| Metric             | Value    |
| ------------------ | -------- |
| R² Score           | ~0.55    |
| Mean Squared Error | ~6.85e10 |

This means the model explains approximately **54% of the variance in house prices**.

---

# 📈 Model Insights

Feature coefficients indicate how each variable influences house price:

| Feature      | Effect                                       |
| ------------ | -------------------------------------------- |
| sqft_living  | Strong positive impact on price              |
| bathrooms    | Positive correlation                         |
| floors       | Positive correlation                         |
| yr_built     | Older houses slightly decrease price         |
| yr_renovated | Small effect due to many non-renovated homes |

---

# 🛠️ Technologies Used

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Scikit-learn**
* **Jupyter Notebook**

---

# 🚀 Project Structure

```
house-price-prediction/
│
├── house_price_prediction.ipynb
├── README.md
├── requirements.txt
└── data/
    └── kc_house_data.csv
```

---

# 📦 Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/house-price-prediction.git
cd house-price-prediction
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the notebook:

```bash
jupyter notebook
```

---

# 🔮 Future Improvements

Possible improvements for this project:

* Add more features such as **zipcode, location, and view**
* Perform **feature engineering**
* Use **log transformation for price**
* Try more advanced models:

  * Random Forest
  * Gradient Boosting
  * XGBoost
* Perform **hyperparameter tuning**

---

# 📚 What I Learned

Through this project I practiced:

* Building a complete **machine learning pipeline**
* Performing **data exploration and visualization**
* Training and evaluating **regression models**
* Interpreting **model coefficients and performance metrics**

---

# 👨‍💻 Author

Computer Science Student exploring **Machine Learning and Data Science**.

If you found this project interesting, feel free to ⭐ the repository!
