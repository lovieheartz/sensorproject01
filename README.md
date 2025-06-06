# Sensor Fault Detection for Semiconductor Wafers

## Project Overview
This project aims to develop a machine learning model to predict the quality of semiconductor wafers ("Good" or "Bad") based on sensor readings collected during the fabrication process. The goal is to enable early detection of defective wafers, improving yield and reducing waste in semiconductor manufacturing.

## Problem Statement
Semiconductor wafer fabrication is a complex process where defects can occur at various stages. Traditional post-production inspection methods lead to delays and wasted resources. This project addresses these challenges by leveraging real-time sensor data to predict wafer quality early in the production cycle.

### Key Objectives:
- Build a binary classification model to predict wafer quality (Good: `1`, Bad: `-1`).
- Use 590 sensor readings (features) collected during fabrication.
- Enable real-time decision-making to flag faulty wafers or adjust process parameters.

## Dataset
- **Input Features**: 590 sensor readings (e.g., temperature, pressure, gas flow) labeled as `Sensor-1` to `Sensor-590`.
- **Target Variable**: Binary label (`1` for "Good" wafer, `-1` for "Bad" wafer).

## Methodology
1. **Data Preprocessing**:
   - Clean and normalize sensor data.
   - Handle missing values and outliers.
   - Perform feature engineering if needed.

2. **Model Selection**:
   - Logistic Regression (baseline interpretability).
   - Random Forest/Gradient Boosting (complex feature interactions).
   - Neural Networks (large-scale pattern recognition).

3. **Model Training**:
   - Train on historical data with known wafer quality labels.
   - Validate using cross-validation techniques.

4. **Real-Time Deployment**:
   - Integrate the model into the production line for real-time predictions.
   - Flag faulty wafers or trigger process adjustments.

5. **Continuous Improvement**:
   - Monitor model performance and retrain with new data.
   - Implement anomaly detection for sensor/process irregularities.
