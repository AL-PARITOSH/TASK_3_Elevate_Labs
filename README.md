# TASK_3_Elevate_Labs

# Linear Regression Models (Simple & Multiple)

## Objective
This project demonstrates the implementation and understanding of **Simple** and **Multiple Linear Regression** using Python.

## Dataset
The dataset used is `Housing.csv`, which contains housing prices along with various features such as area, bedrooms, bathrooms, stories, and other categorical variables.

## Tools & Libraries
- **Pandas**: Data handling and preprocessing.  
- **Scikit-learn**: Model training and evaluation.  
- **Matplotlib**: Data visualization.  

## Steps Followed

### 1. Import and Preprocess the Dataset
- Loaded the dataset using Pandas.  
- Converted categorical variables into dummy/indicator variables using `pd.get_dummies()`.  

### 2. Split Data into Train-Test Sets
- Used `train_test_split` from `sklearn.model_selection` to split into training and testing sets.

### 3. Fit a Linear Regression Model
- **Simple Linear Regression**: `price` vs `area`.  
- **Multiple Linear Regression**: `price` vs all features.

### 4. Evaluate the Model
- Metrics used:  
  - **MAE** (Mean Absolute Error)  
  - **MSE** (Mean Squared Error)  
  - **R² Score**

### 5. Plot Regression Line & Interpret Coefficients
- Plotted the regression line for the **Simple Linear Regression** model.  
- Interpreted slope (coefficient) and intercept values.

## Results Summary
| Model | MAE | MSE | R² Score |
|-------|------|------|----------|
| Simple Linear Regression | ~1.47M | ~3.68e12 | ~0.27 |
| Multiple Linear Regression | ~0.97M | ~1.75e12 | ~0.65 |

- **Interpretation**:  
  - Multiple Linear Regression performed better (higher R² and lower errors).  
  - In Simple LR, the coefficient for `area` (~425) indicates that **for each additional square unit of area, price increases by ~425 units**.

## How to Run
1. Place `Housing.csv` in the same directory as the notebook.  
2. Install required libraries:  
   ```bash
   pip install pandas scikit-learn matplotlib
