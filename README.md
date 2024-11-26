# Activity Classification Project

## Overview
This project focuses on classifying human activities using sensor data from wearable devices. The dataset contains measurements from various sensors capturing different physical activities performed by multiple subjects.

## Dataset Description
- **Source**: [Daily and Sports Activities Dataset](https://archive.ics.uci.edu/dataset/256/daily+and+sports+activities) [1]
- **Important**: Download the dataset ZIP file from the source link and save it as `daily_and_sports_activities.zip` in the project root directory
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

## Setup Instructions
1. Download the [Daily and Sports Activities Dataset](https://archive.ics.uci.edu/dataset/256/daily+and+sports+activities) ZIP file
2. Save the downloaded file as `daily_and_sports_activities.zip` in the project root directory
3. Install required dependencies:
   ```bash
   pip install pandas numpy scikit-learn
   ```
4. Run the Jupyter notebook `Activity_Classification.ipynb` to process the data and train the models

## Contributors
- Evan Scott
- Deepti
- Ajmal Jalal

## References
[1] Barshan, B. & Altun, K. (2010). Daily and Sports Activities [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5C59F.