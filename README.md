# effective-malaria-detection

## Overview
This project addresses the issue of data leakage in malaria detection using Convolutional Neural Networks (CNN). We identified that previous works in this domain often suffer from data leakage due to the same patient's data appearing in both training and testing sets. To mitigate this, we introduced a new dataset split strategy, ensuring that data from a single patient is restricted to either the training or testing set.

### Key Features
- Recreated previously published models to identify data leakage.
- Trained multiple models (scratch, transfer learning, ensemble learning) on a patient-wise split dataset.
- Applied float16 and int8 quantization using PyTorch for optimized model performance.
- Comprehensive analysis of model performance, highlighting improvements with the corrected dataset.

## Directory Structure
- `data/`: Contains raw and processed datasets, including patient-wise split data.
- `models/`: Includes implementations of recreated models, trained models, and quantized versions.
- `notebooks/`: Jupyter notebooks for data analysis, training, and evaluation.
- `src/`: Source code for data processing, model training, and evaluation.
- `results/`: Analysis results and visualizations of model performance.
- `tests/`: Unit tests for data processing, model training, and evaluation scripts.
- `docs/`: Documentation and reports on findings, methodologies, and visualizations.

## Installation
To set up the project environment, install the required dependencies using:
```bash
pip install -r requirements.txt
```

## Usage
- Follow the data preprocessing steps in the notebooks/data_analysis.ipynb.
- Train models using the notebooks/model_training.ipynb.
- Evaluate model performance with the notebooks/model_evaluation.ipynb.
- Quantize the models using the notebooks/quantization.ipynb.

## License
This project is licensed under the [Apache License 2.0](LICENSE) - see the [LICENSE](LICENSE) file for details.


