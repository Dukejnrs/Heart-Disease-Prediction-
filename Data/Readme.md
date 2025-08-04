# Data Folder

This folder contains data-related files for the Heart Disease Prediction project.

The dataset is fetched automatically from the UCI Machine Learning Repository using the `ucimlrepo` Python package.

No CSV files are stored here to keep the repository lightweight and reproducible.

To fetch the dataset:

```python
from ucimlrepo import fetch_ucirepo

heart_disease = fetch_ucirepo(id=45)
X = heart_disease.data.features
y = heart_disease.data.targets
