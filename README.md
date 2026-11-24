# Zomato Restaurant Rating Prediction

An end-to-end machine learning project that investigates restaurant ratings using Zomato data. The notebook covers data cleaning, exploratory analysis, feature engineering, model comparison, and evaluation.

## Project questions

- How do ratings vary across cuisines, locations, and price ranges?
- Which features help classify restaurant ratings?
- How can repeated restaurants affect evaluation, and how should data leakage be reduced?

## Method

1. Clean and validate the tabular data.
2. Explore rating, cuisine, location, and pricing patterns with visualizations.
3. Prepare features for classification and compare seven models.
4. Evaluate models with accuracy, precision, recall, F1-score, and ROC-AUC.
5. Address repeated restaurant entries by splitting at restaurant level to reduce leakage between train and test data.

## Tools

Python · Pandas · NumPy · Matplotlib · Seaborn · Scikit-learn · Jupyter

## Run the notebook

```bash
git clone https://github.com/MohamedAtefAbdelwhab/Zomatoo.git
cd Zomatoo
pip install -r requirements.txt
jupyter notebook "Zomatoo .ipynb"
```

The dataset is not included in this repository. Update the data path in the notebook to point to your local copy before running it.

## Repository contents

- [`Zomatoo .ipynb`](./Zomatoo%20.ipynb) — analysis, feature preparation, model comparison, and evaluation
- [`requirements.txt`](./requirements.txt) — Python dependencies

## Evaluation note

Repeated entries for the same restaurant can make a random row split overly optimistic. This project uses restaurant-level splitting so that records for a restaurant do not appear in both training and test sets.

## Author

[Mohamed Atef](https://github.com/MohamedAtefAbdelwhab)