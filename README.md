# Heart Failure Survival Analysis

**Michigan Data Science Team | Winter 2026**

Project Leads: Sina Bonakdar & Terry Zhang

---

## Executive Summary

Survival analysis of heart failure patients is critical for identifying key factors that distinguish survival from mortality. This project provides a comprehensive, hands-on learning experience in clinical data science.

Through this tutorial series, students will:

- Implement **visualization tools** to extract meaningful insights from clinical data
- Apply **statistical and analytical methods** to understand feature relationships
- Build **machine learning and deep learning classifiers** to predict patient outcomes
- Evaluate model performance using **multiple evaluation metrics**

**Key Finding**: By the end of this project, students will discover that only **two features** are sufficient to distinguish survival from death using various classifiers.

---

## Project Structure

| Week | Topic | Description | Key Concepts |
|------|-------|-------------|--------------|
| 1 | Data Exploration | Dataset overview, visualization, and initial insights | Pandas, Seaborn, Matplotlib, EDA |
| 2 | Statistical Analysis | Hypothesis testing, correlation, and feature importance | T-test, Mann-Whitney U, FDR, Random Forest |
| 3 | Feature Engineering | Feature selection and transformation | VIF, Scaling, Encoding |
| 4 | Machine Learning | Classification models and evaluation | Logistic Regression, SVM, Decision Trees |
| 5 | Deep Learning | Neural network classifiers | TensorFlow/PyTorch, MLP |
| 6 | Final Analysis | Model comparison and key findings | ROC-AUC, Precision-Recall, Feature Analysis |

---

## Dataset

**Heart Failure Clinical Records Dataset**
- 299 patients with heart failure
- 13 clinical features including age, ejection fraction, serum creatinine
- Binary outcome: survival or death during follow-up

Source: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Heart+failure+clinical+records)

---

## Resources

### Statistical Analysis
- [Scipy Stats Documentation](https://docs.scipy.org/doc/scipy/reference/stats.html)
- [Statsmodels Guide](https://www.statsmodels.org/stable/index.html)

### Machine Learning
- [Scikit-learn Documentation](https://scikit-learn.org/stable/)
- [Feature Selection Techniques](https://scikit-learn.org/stable/modules/feature_selection.html)

### Deep Learning
- [TensorFlow Tutorials](https://www.tensorflow.org/tutorials)
- [PyTorch Documentation](https://pytorch.org/docs/stable/index.html)

### Research Paper
- Chicco, D., Jurman, G. *Machine learning can predict survival of patients with heart failure*. BMC Med Inform Decis Mak 20, 16 (2020)

---

## Getting Started

```bash
# Clone the repository
git clone https://github.com/MichiganDataScienceTeam/W26-MDST-Project_Heart-Failure-Survival-Analysis.git

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter
jupyter notebook
```

---

## License

This project is for educational purposes as part of the Michigan Data Science Team curriculum.
