# ML Project 1: Solubility Prediction

**Author**: Lewi Alemayehu  
**Institution**: University of Washington

---

## Project Overview

This project aims to predict the aqueous solubility (logS) of chemical compounds using machine learning models. The dataset contains molecular descriptors, and the target variable is the logarithmic solubility (logS) of the compounds.

### Objective:
- Develop machine learning models to predict solubility (logS) using features derived from molecular descriptors.
- Evaluate the performance of two models: **Linear Regression** and **Random Forest Regressor**.

---

## Dataset

The dataset used in this project is available from the following source:

- **Data Source**: [Delaney Solubility Dataset](https://raw.githubusercontent.com/dataprofessor/data/master/delaney_solubility_with_descriptors.csv)

### Features:
- Various molecular descriptors used as input features for the machine learning models.

### Target:
- **logS**: The aqueous solubility of the chemical compounds.

---

## Project Structure

- **Data Loading**: The dataset is loaded using pandas.
- **Data Preparation**: The target variable (`logS`) is separated from the feature set.
- **Model Building**: Two machine learning models are trained on the dataset.
  - **Linear Regression**
  - **Random Forest Regressor**
- **Evaluation**: Both models are evaluated using the Mean Squared Error (MSE) and R² metrics on both training and test sets.

---

## Key Steps

1. **Loading Data**: The dataset is loaded from a CSV file into a pandas DataFrame.

2. **Data Preparation**:
   - **X**: Features (molecular descriptors).
   - **y**: Target variable (`logS`).

3. **Data Splitting**: The data is split into training and test sets using an 80/20 split.

4. **Model Training**:
   - **Linear Regression**: A simple linear model is trained on the data.
   - **Random Forest Regressor**: A more complex ensemble model is trained using decision trees.

5. **Model Evaluation**:
   The performance of both models is evaluated using:
   - **Mean Squared Error (MSE)**
   - **R² Score**

---

## Results

Both models are compared based on their performance on the training and test sets. The results are displayed in a DataFrame format for easy comparison.

---

## How to Run the Project

1. Clone the repository.
2. Install the required libraries:
   ```bash
   pip install pandas scikit-learn
