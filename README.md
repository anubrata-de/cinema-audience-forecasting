<!-- portfolio
title: Cinema Audience Forecasting Challenge
tagline: Time Series Prediction
category: Machine learning
summary: Forecasts daily audience counts across theatres from booking, theatre and calendar data. Random Forest scored best (validation R² 0.51) and anchors a three-model ensemble.
tags: Python, scikit-learn, XGBoost, Time series
slug: cinema-audience-forecasting
-->

# Cinema Audience Forecasting Challenge

*Time Series Prediction*

A model that forecasts daily audience counts for multiple theatres, built for a machine learning Kaggle challenge at IIT Madras (Term 3, 2025).

## Approach

- Combined several sources: theatre metadata, bookings from online platforms and on-site point-of-sale systems, and calendar information such as weekends and holidays.
- Compared original, PCA and selected feature sets, then a range of regression models: Ridge, ElasticNet, KNN, Random Forest, Extra Trees, Gradient Boosting, XGBoost and LightGBM.
- Combined the three strongest models into an ensemble for the final forecasts.

## Results (validation)

- **Random Forest** was the best single model: **R² 0.51, RMSE 22.2** audience members per day.
- Feature choice mattered more than the model. Ridge only worked after PCA (R² −135 on raw features, 0.43 with PCA).

## Files

- [`cinema_audience_forecasting.ipynb`](cinema_audience_forecasting.ipynb): the full Kaggle notebook, with code and outputs.

---

Part of the BS in Data Science and Applications at IIT Madras. More projects: [anubrata.vercel.app](https://anubrata.vercel.app/projects).
