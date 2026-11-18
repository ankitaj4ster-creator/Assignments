# Comparing Classifiers: Bank Marketing

A machine-learning analysis that predicts whether a Portuguese bank customer will subscribe to a term deposit. The project applies CRISP-DM and compares Logistic Regression, K-Nearest Neighbors, Decision Tree, and Support Vector Machine classifiers.

## Project Overview

The analysis uses the UCI Bank Marketing dataset (`bank-additional-full.csv`) containing 41,188 customer contacts. It compares model performance, inspects the impact of feature groups, and avoids the post-call `duration` variable to prevent data leakage.

Key findings:

- Always predicting "no" produces 88.7% accuracy, so accuracy alone is misleading.
- Client-profile features alone have limited predictive value.
- Campaign history, timing, contact context, and macro-economic variables improve ranking performance.
- Tuned Logistic Regression provides strong, interpretable, and efficient performance.
- Ranking the top 20% of customers captures approximately two-thirds of likely subscribers.

## Repository Contents

- `Comparing_Classifiers_Bank_Marketing.ipynb` — full notebook with analysis, visualizations, model training, and evaluation
- `README.md` — project documentation

## Models Compared

- Logistic Regression
- K-Nearest Neighbors
- Decision Tree
- Support Vector Machine

Evaluation includes accuracy, recall, ROC-AUC, PR-AUC, and lift/ranking analysis.

## Getting Started

### Requirements

- Python 3.9 or newer
- Jupyter Notebook or JupyterLab
- pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- scikit-learn

Install the dependencies:

```bash
pip install notebook pandas numpy matplotlib seaborn scipy scikit-learn
```

### Run the Notebook

1. Clone this repository.
2. Place `bank-additional-full.csv` in a `data/bank-additional/` folder, or place it beside the notebook.
3. Open the notebook:

```bash
jupyter notebook Comparing_Classifiers_Bank_Marketing.ipynb
```

## Data Source

Moro, Cortez, and Rita, *A Data-Driven Approach to Predict the Success of Bank Telemarketing*, UCI Machine Learning Repository, 2014.

Dataset: [Bank Marketing](https://archive.ics.uci.edu/dataset/222/bank+marketing)

## Methodology

The notebook follows CRISP-DM:

1. Business understanding
2. Data understanding
3. Data preparation
4. Modeling
5. Evaluation
6. Deployment recommendations

## License

This project is provided for educational purposes. The dataset is governed by its source license and terms.
