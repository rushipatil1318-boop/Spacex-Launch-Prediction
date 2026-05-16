# SpaceX Falcon 9 First Stage Landing Prediction

Built a machine learning classification model to predict whether 
SpaceX Falcon 9's first stage will successfully land after launch. 
Reusable rockets are central to reducing launch costs — predicting 
landing success helps estimate mission cost and feasibility.

## Business Problem

SpaceX charges around $62 million per launch compared to competitors 
charging $165 million+. The cost advantage comes from reusing the 
first stage. Predicting whether a booster will land successfully 
helps estimate true mission cost and supports competitive pricing 
decisions for commercial space customers.

## What I did

- Collected launch data using SpaceX REST API and web scraping
- Cleaned and prepared the dataset — handled missing values, 
  encoded categorical features, normalized numerical inputs
- Performed exploratory analysis on launch sites, payload mass, 
  orbit types, and booster versions
- Built and compared multiple classification models
- Evaluated using accuracy, confusion matrix, and F1 score

## Models Compared

| Model | Accuracy |
|---|---|
| Logistic Regression | 83% |
| Decision Tree | 87% |
| SVM | 83% |
| KNN | 83% |

Decision Tree performed best on the test set.

## Key Findings

- Launch success rate improved significantly after 2015 as 
  SpaceX refined landing techniques
- KSC LC-39A launch site has the highest success rate
- Higher payload mass correlates with lower landing success 
  probability
- LEO and ISS orbits show consistently higher landing success rates

## Tools

Python · Pandas · NumPy · Scikit-learn · Matplotlib · Seaborn · 
Folium · Plotly · SQL · REST API

## How to Run

```bash
pip install pandas numpy scikit-learn matplotlib seaborn folium plotly
jupyter notebook SpaceX_Landing_Prediction.ipynb
```# Spacex-Launch-Prediction
