# Medical Insurance Premium Predictor & Risk Profiler

An interactive machine learning pipeline that predicts medical charges and classifies patient risk based on demographic and clinical factors. This project implements linear regression with custom feature engineering, logistic regression classifier for smoking detection, and interactive slider calculators built using Jupyter widgets.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hFi_DZSdEpNXLD4wnRXgYn_4UqKUT977#scrollTo=d6201c4b)

## Key Insights & Business Findings
- **The Obesity-Smoking Multiplier**: Having both a BMI $\ge$ 30 and being a smoker compounds risk dramatically. The high-risk group faces extreme costs with a historical median charge exceeding **$40,900**.
- **Smoker Classification**: We can predict whether a person is a smoker with **96.64% accuracy** using other medical metrics (such as age, BMI, and overall charges) via a Logistic Regression model.
- **Feature Engineering Lift**: Adding a custom interaction term (`bmi_smoker`) to our Linear Regression model improved the $R^2$ score from **0.7836** to **0.8653** and dropped the prediction error (RMSE) from **$5,796.28** to **$4,573.81**.

## Tech Stack & Libraries
- **Language**: Python 3
- **Data Analysis & Visualization**: Pandas, NumPy, Seaborn, Matplotlib
- **Machine Learning**: Scikit-Learn (Linear Regression, Logistic Regression, Train-Test Split, Regression & Classification Metrics)
- **Interactive UI**: `ipywidgets` (Sliders, Buttons, and Dynamic Calculation Panels)

## How to Run the Project
1. Click the **Open in Colab** badge at the top of this page.
2. Upload the `insurance.csv` file to your Colab temporary workspace folder.
3. Run all cells (`Runtime > Run all` or `Ctrl + F9`).
4. Use the **Interactive Smoker Predictor** or the **Interactive Risk Profile Calculator** sliders at the bottom to predict real-time insurance profiles!
