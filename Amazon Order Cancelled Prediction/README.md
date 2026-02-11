# 📦 Amazon Order Delay Prediction 🚚

## 🎯 Project Objective

The goal of this project is to build a predictive model that identifies whether an order will be **Delayed** or  **Cancelled** . By leveraging historical Amazon sales data, we aim to help logistics teams proactively manage customer expectations and optimize delivery routes.

---

## 📂 Project Structure

* **`Amazon.csv`** 📊: The raw dataset containing 100,000 order records.
* **`train_model.ipynb`** 📓: Jupyter Notebook containing the data cleaning, feature engineering, and model training logic.

---

## 🔍 Dataset Features

The model analyzes several key factors to predict the order status:

* **Financials** 💰: `UnitPrice`, `Discount`, `ShippingCost`, `TotalAmount`.
* **Logistics** 🚛: `Quantity`, `Category`, `PaymentMethod`.
* **Geography** 🌍: `Country`, `State`, `City`.
* **Target Variable** 🎯: `OrderStatus` (Converted to binary for delay/cancellation prediction).

---

## 🛠️ Technical Workflow

### 1️⃣ Data Preprocessing

* **Cleaning** : Removed null entries and unnecessary identifiers (`OrderID`, `CustomerID`).
* **Label Encoding** : Categorical variables like **Payment Method** and **Category** were converted into numerical format for the model.
* **Splitting** : Used an 80/20 train-test split to ensure unbiased evaluation.

### 2️⃣ Machine Learning Model

We utilized a **Random Forest Classifier** 🌲 due to its robustness against outliers and its ability to handle non-linear relationships in e-commerce data.

**Python**

```
# Model initialization
model = RandomForestClassifier(random_state=42)
model.fit(X_train, y_train)
```

### 3️⃣ Results

* **Accuracy Score** ✅: **96.06%**
* The model shows high precision in distinguishing between successful deliveries and potential disruptions.
