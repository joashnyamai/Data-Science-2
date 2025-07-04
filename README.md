# 🚧 Road Accident Severity Prediction Using Linear Regression

This project uses a linear regression model to predict road accident severity based on road and environmental factors. It demonstrates how data-driven approaches can help governments, especially in underdeveloped countries, reduce traffic-related risks.

## 📁 Dataset
A custom dataset `road_accidents.csv` with features:
- `Speed_limit`
- `Weather_conditions`
- `Time_of_day`
- `Number_of_vehicles_involved`
- `Accident_Severity` (target variable)

## 🧪 Model
Built using **Python (scikit-learn)**:
- Model: `LinearRegression`
- Split: 80% training, 20% testing
- Evaluation: Mean Squared Error (MSE)

## 📌 Features Used
- Speed Limit (km/h)  
- Weather Conditions (coded: 1=sunny, 2=rainy, 3=foggy)  
- Time of Day (24-hour format)  
- Number of Vehicles Involved

## 🔍 Prediction Example
```python
sample = pd.DataFrame({
    'Speed_limit': [60],
    'Weather_conditions': [2],
    'Time_of_day': [15],
    'Number_of_vehicles_involved': [3]
})
predicted = model.predict(sample)
