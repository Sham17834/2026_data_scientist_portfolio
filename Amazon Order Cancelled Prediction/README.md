# 📦 Order Cancellation Prediction (Machine Learning)

## 📌 Project Overview

This project builds a simple machine learning model to predict whether an Amzon order will be **Delivered** or **Cancelled** based on historical transaction data.

The goal is to demonstrate a beginner-friendly, applied AI workflow including data cleaning, feature encoding, model training, and evaluation using Python and scikit-learn.

---

## 🎯 Objective

Predict `OrderStatus`:

* 0 → Delivered
* 1 → Cancelled

This can help businesses identify risky orders early and take preventive actions.

---

## 🧠 Technologies Used

* Python
* pandas
* scikit-learn
* Jupyter Notebook / VS Code

---

## 📂 Dataset

* 100,000 e-commerce order records
* Features include product details, pricing, discounts, payment method, country, and shipping cost.

Selected columns:

* Quantity
* UnitPrice
* Discount
* ShippingCost
* TotalAmount
* Category
* PaymentMethod
* Country
* OrderStatus

---

## 🔄 Workflow

1. Load dataset
2. Keep relevant columns
3. Remove missing values
4. Encode categorical features
5. Split data into training and testing sets
6. Train Random Forest classifier
7. Evaluate model accuracy

---

## 🤖 Model

* Random Forest Classifier (scikit-learn)

---

## 📈 Result

The model achieves around 96% **accuracy** in predicting whether an order will be cancelled or delivered.
