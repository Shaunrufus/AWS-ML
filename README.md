# AWS-ML


# AWS SageMaker XGBoost ML Pipeline

This project demonstrates the complete machine learning pipeline using **Amazon SageMaker Studio** with **XGBoost** for predicting insurance charges based on customer attributes.

---

##  Project Overview

- **Algorithm Used:** XGBoost Regressor (in-built estimator from AWS)
- **Use-case:** Predicting medical insurance charges
- **Platform:** AWS SageMaker Studio
- **Dataset:** `insurancecharges.csv` (includes age, sex, smoker status, region, etc.)

---

##  ML Pipeline Components

| Step                 | Description                                                                 |
|----------------------|-----------------------------------------------------------------------------|
| 1. Data Upload       | Uploaded to **Amazon S3** in train/test split.                              |
| 2. Data Preprocessing| Handled categorical encoding, missing values (if any).                      |
| 3. Model Loading     | Loaded in-built XGBoost model from `model.tar.gz` (AWS trained model).      |
| 4. Inference         | Performed predictions using `Booster` object locally.                       |
|
