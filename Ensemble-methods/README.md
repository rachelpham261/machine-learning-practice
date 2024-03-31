# Income Classification With Ensemble Methods

This repository implements different ensemble methods (Random Forest, AdaBoost, Gradient Boost, XGB) for classifying individuals into 2 income categories, > 50K and < 50K. The code for processing the data, training, evaluation, and hyperparameter tunining is included in the notebook `ensemble.ipynb`.

## Usage

Run the code blocks in `ensemble.ipynb` sequentially for data processing, training, evaluating the model with various metrics, and hyperparameter tunining.

## Required packages
The code requires `pandas` for reading and processing data, `sklearn` and `xgboost` for the implementation of different ensemble methods. `seaborn` and `matplotlib` are also needed for visualization.

## Software/Library versions
- Python: 3.11.5
- Pandas: 1.26.3
- Sklearn: 1.2.2
- Xgboost: 2.0.3
- Seaborn: 0.13.1
- Matplotlib: 3.8.0