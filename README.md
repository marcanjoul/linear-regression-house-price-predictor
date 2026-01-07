# House Price Predictor (Linear Regression)

This project demonstrates the fundamentals of **single-variable linear regression** using Python and scikit-learn.  
The goal is to understand how a simple machine learning model learns the relationship between **house area** and **price**, and how it can be used to make predictions on new data.

---

## Project Overview

- **Input (Feature):** House area (square feet)
- **Output (Target):** House price (USD)
- **Model:** Linear Regression
- **Dataset:** Synthetic CSV created for learning purposes

This project intentionally uses a **clean, simple dataset** to focus on core ML concepts before moving on to real-world, noisy data.

---

## What This Project Covers

- Loading CSV data with pandas
- Visualizing data using scatter plots
- Training a linear regression model
- Interpreting slope and intercept
- Making predictions for new inputs
- Exporting predictions to a CSV file

---

## Example Visualization

The model learns a linear relationship between area and price:

- Red points: actual data
- Blue line: fitted regression line

This helps visualize how the model approximates the trend in the data.

---

## Making Predictions

The trained model is applied to new area values from areas.csv, and predictions are saved to prediction.csv:

```python
predictions = reg.predict(new_data)
```
This simulates how a trained ML model can be reused on unseen data.


## Model Training

The model is trained using scikit-learn:

```python
from sklearn.linear_model import LinearRegression

reg = LinearRegression()
reg.fit(df[['area']], df['price'])
```
---

## Notes & Limitations

- This is a learning-focused project, not a production-ready price predictor.
- Real house prices depend on many features (location, bedrooms, amenities, etc.).
- Single-variable linear regression is used here as a foundational step.

---

## Technologies Used
- Python
- pandas
- numpy
- matplotlib
- scikit-learn

---

## How to add it to your repo

```bash
touch README.md
# paste the content above
git add README.md
git commit -m "Add project README explaining linear regression workflow"
git push
```
