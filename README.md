# MLUsingPython: End-to-End Machine Learning Workflows

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.3+-orange.svg)](https://scikit-learn.org/)
[![pandas](https://img.shields.io/badge/pandas-2.0+-blue.svg)](https://pandas.pydata.org/)
[![matplotlib](https://img.shields.io/badge/matplotlib-3.6+-blue.svg)](https://matplotlib.org/)

A comprehensive collection of end-to-end machine learning workflows demonstrating different ML algorithms on various types of data. Perfect for learning ML concepts through practical implementations.

## 📋 Table of Contents

- [Project Overview](#project-overview)
- [Project Structure](#project-structure)
- [Machine Learning Models Covered](#machine-learning-models-covered)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Notebooks Overview](#notebooks-overview)
- [Key Findings](#key-findings)
- [Learning Outcomes](#learning-outcomes)
- [Contributing](#contributing)

## 🎯 Project Overview

This repository contains two complete machine learning workflows that demonstrate:

1. **Classification**: Iris flower species prediction using multiple classification algorithms
2. **Regression**: California housing price prediction using multiple regression algorithms

Each workflow follows a complete ML pipeline: data exploration → preprocessing → model training → evaluation → comparison → insights.

## 📁 Project Structure

```
MLUsingPython/
│
├── IrisClassification/
│   ├── Iris.csv                    # Iris dataset (alternative to seaborn)
│   └── IrisClassification.ipynb    # Classification workflow notebook
│
├── housing_predition_regression/
│   ├── california_housing_train.csv    # Training data (17,000 samples)
│   ├── california_housing_test.csv     # Test data (3,000 samples)
│   └── housing_prediction.ipynb         # Regression workflow notebook
│
└── README.md                       # This file
```

## 🤖 Machine Learning Models Covered

### Classification Models (Iris Dataset)
- **Logistic Regression** - Linear classification algorithm
- **Decision Tree** - Tree-based classifier
- **Support Vector Machine (SVM)** - Kernel-based classifier
- **K-Nearest Neighbors (KNN)** - Distance-based classifier
- **Naive Bayes** - Probabilistic classifier
- **Gradient Boosting** - Ensemble boosting classifier
- **Random Forest** - Ensemble bagging classifier

### Regression Models (California Housing Dataset)
- **Linear Regression** - Simple linear model
- **Ridge Regression** - L2 regularized linear model
- **Lasso Regression** - L1 regularized linear model
- **Random Forest Regressor** - Ensemble tree regressor
- **Gradient Boosting Regressor** - Sequential boosting regressor
- **Support Vector Regression (SVR)** - Kernel-based regressor
- **K-Nearest Neighbors Regressor** - Distance-based regressor

## 📋 Prerequisites

- Python 3.8 or higher
- Jupyter Notebook or JupyterLab
- Basic understanding of Python and machine learning concepts

## 🚀 Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/harsh64patel/MLUsingPython.git
   cd MLUsingPython
   ```

2. **Create a virtual environment (recommended):**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install required packages:**
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```

4. **Start Jupyter Notebook:**
   ```bash
   jupyter notebook
   ```

## 📖 Usage

### Running the Classification Notebook
1. Navigate to `IrisClassification/` directory
2. Open `IrisClassification.ipynb`
3. Run cells sequentially to see the complete workflow
4. Compare 7 different classification algorithms

### Running the Regression Notebook
1. Navigate to `housing_predition_regression/` directory
2. Open `housing_prediction.ipynb`
3. Run cells sequentially to see the complete workflow
4. Compare 7 different regression algorithms

## 📊 Notebooks Overview

### 1. Iris Classification (`IrisClassification.ipynb`)

**Dataset**: Iris flower dataset (150 samples, 4 features, 3 classes)
- Features: sepal_length, sepal_width, petal_length, petal_width
- Target: species (setosa, versicolor, virginica)

**Workflow**:
- Data loading and exploration
- Feature visualization with pair plots
- Data preprocessing and train/test split
- Training 7 classification models
- Performance comparison and visualization
- Confusion matrix analysis
- Accuracy comparison charts

### 2. California Housing Price Prediction (`housing_prediction.ipynb`)

**Dataset**: California housing dataset (20,000 samples, 8 features + target)
- Features: longitude, latitude, housing_median_age, total_rooms, total_bedrooms, population, households, median_income
- Target: median_house_value

**Workflow**:
- Data loading and comprehensive exploration
- Statistical analysis and correlation matrix
- Feature scaling and preprocessing
- Training 7 regression models
- Multi-metric evaluation (RMSE, MAE, R², MAPE)
- Performance visualization and comparison
- Residual analysis
- Model recommendations

## 🏆 Key Findings

### Classification Results (Iris Dataset)
- **All models achieved 100% accuracy** on the test set
- This demonstrates the dataset's well-separated classes
- Models like SVM, Random Forest, and Gradient Boosting showed robust performance

### Regression Results (California Housing Dataset)
- **Best Model**: Random Forest Regressor
  - R² Score: 0.8088 (explains 80.88% of variance)
  - RMSE: $49,458 (average prediction error)
  - MAE: $32,191 (mean absolute error)

- **Performance Ranking** (by R² Score):
  1. Random Forest (0.8088)
  2. Gradient Boosting (0.7617)
  3. KNN Regressor (0.6899)
  4. Linear/Ridge/Lasso Regression (0.6195)
  5. SVR (0.3045)

## 🎓 Learning Outcomes

After working through these notebooks, you'll understand:

### Data Science Fundamentals
- Data exploration and visualization techniques
- Feature engineering and preprocessing
- Train/test split and cross-validation concepts

### Machine Learning Concepts
- Different types of ML algorithms (linear, tree-based, distance-based)
- Model evaluation metrics for classification and regression
- Bias-variance tradeoff
- Ensemble learning methods

### Practical Skills
- Implementing ML workflows in Python
- Using scikit-learn effectively
- Model comparison and selection
- Result interpretation and visualization

### Algorithm-Specific Knowledge
- When to use different algorithms
- Hyperparameter importance
- Computational complexity considerations
- Interpretability vs. accuracy tradeoffs

## 🤝 Contributing

This repository is designed for learning purposes. Feel free to:

- **Improve the code**: Add better visualizations, error handling, or documentation
- **Add new models**: Implement additional ML algorithms
- **Enhance workflows**: Add feature engineering, hyperparameter tuning, or cross-validation
- **Create tutorials**: Add explanations for specific concepts
- **Report issues**: Found a bug or have suggestions?

### How to Contribute
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📚 Additional Resources

### Recommended Learning Path
1. **Python Basics**: Learn Python fundamentals
2. **Data Analysis**: Master pandas and numpy
3. **Visualization**: Learn matplotlib and seaborn
4. **Machine Learning**: Study scikit-learn documentation
5. **Statistics**: Understand evaluation metrics

### Useful Links
- [Scikit-learn Documentation](https://scikit-learn.org/stable/documentation.html)
- [Python Data Science Handbook](https://jakevdp.github.io/PythonDataScienceHandbook/)
- [Machine Learning Mastery](https://machinelearningmastery.com/)
- [Towards Data Science](https://towardsdatascience.com/)

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

**Happy Learning! 🚀**

If you find this repository helpful, please give it a ⭐ star!
