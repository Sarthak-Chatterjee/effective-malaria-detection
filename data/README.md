# Data Directory

## Overview
The `data/` directory contains the datasets used in this project for malaria detection, including the raw data, processed data, and patient-wise split data.

### Structure
- `raw/`: The unprocessed original dataset.
- `processed/`: Cleaned and preprocessed data, ready for model training.
- `patient_wise_split/`: Data organized to prevent leakage by ensuring patient data does not appear in both training and testing sets.

## Instructions
1. Place the original datasets in the `raw/` folder.
2. Use the `notebooks/data_analysis.ipynb` to preprocess and generate the `processed/` and `patient_wise_split/` datasets.