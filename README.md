# Activity Classification Project

## Overview
This project focuses on classifying human activities using sensor data from wearable devices. The dataset contains measurements from various sensors capturing different physical activities performed by multiple subjects.

## Dataset Description
- **Source**: Daily and Sports Activities Dataset
- **Activities**: 19 different activities including:
  - Sitting
  - Standing
  - Lying on Back
  - Lying on Right Side
  - Ascending Stairs
  - Descending Stairs
  - Standing in Elevator
  - Moving in Elevator
  - Walking in Parking Lot
  - Walking on Treadmill (Flat)
  - Walking on Treadmill (Inclined)
  - Running on Treadmill
  - Exercising on Stepper
  - Exercising on Cross Trainer
  - Cycling (Horizontal)
  - Cycling (Vertical)
  - Rowing
  - Jumping
  - Playing Basketball

## Data Processing
- Original data contains sensor measurements sampled at 25Hz over 5-second windows
- Features reduced to 1-second segments to prevent overfitting
- Data normalized using StandardScaler
- Dataset split into training (80%) and test (20%) sets
- Total instances: 9,120
- Features per instance: 1,125

## Project Structure
- `Activity_Classification.ipynb`: Main notebook containing data processing and analysis
- Data preprocessing steps include:
  - Extraction of sensor data
  - Feature flattening
  - Normalization
  - Train-test splitting

## Dependencies
- Python 3.x
- pandas
- numpy
- scikit-learn