# Backend API

Python API for connecting the EAMS application with the machine learning model.

## Responsibilities

- Load the trained ML model
- Receive sensor readings
- Validate incoming data
- Prepare input for prediction
- Generate the screening risk level
- Return prediction results to the application

## Planned Flow

Sensor Data
↓
Python API
↓
Data Validation
↓
ML Model
↓
Risk Prediction
↓
API Response

## Output

The API will return a screening risk category such as:

- Lower Risk
- Further Assessment
- Higher Risk

The output is intended for screening support and not medical diagnosis.