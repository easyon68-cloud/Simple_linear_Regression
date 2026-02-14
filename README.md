# Simple_linear_Regression
A machine learning project implementing Simple Linear Regression to predict sales based on TV advertising spend using the Advertising dataset.


# Simple Linear Regression - Sales Prediction

A machine learning project implementing Simple Linear Regression to predict sales based on TV advertising spend using the Advertising dataset.

## 📋 Project Overview

This project demonstrates the implementation of Simple Linear Regression to analyze the relationship between TV advertising expenditure and product sales. The model predicts sales figures based on TV advertising budget, providing insights into advertising effectiveness.

## 🎯 Objectives

- Understand the relationship between TV advertising spend and sales
- Build a Simple Linear Regression model from scratch
- Evaluate model performance using appropriate metrics
- Visualize the regression line and predictions

## 📊 Dataset

**Dataset:** Advertising.csv

**Features:**
- `TV`: TV advertising budget (in thousands of dollars)
- `Radio`: Radio advertising budget (in thousands of dollars)
- `Newspaper`: Newspaper advertising budget (in thousands of dollars)
- `Sales`: Product sales (in thousands of units)

**Note:** This project uses only the `TV` feature for Simple Linear Regression.

## 🛠️ Technologies Used

- **Python 3.x**
- **Libraries:**
  - `pandas` - Data manipulation and analysis
  - `numpy` - Numerical computations
  - `matplotlib` - Data visualization
  - `seaborn` - Statistical data visualization
  - `scikit-learn` - Machine learning model implementation

## 📁 Project Structure

```
simple-linear-regression/
│
├── Simple_linear_Regression__1_.ipynb    # Main Jupyter notebook
├── Advertising.csv                        # Dataset (not included)
└── README.md                              # Project documentation
```

## 🚀 Getting Started

### Prerequisites

Install required packages:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### Running the Project

1. Clone this repository:
```bash
git clone https://github.com/yourusername/simple-linear-regression.git
cd simple-linear-regression
```

2. Upload your `Advertising.csv` dataset to the appropriate directory

3. Open the Jupyter notebook:
```bash
jupyter notebook Simple_linear_Regression__1_.ipynb
```

4. Run all cells sequentially

## 📝 Implementation Steps

### Step 1: Import Libraries
Import necessary Python libraries for data handling, visualization, and machine learning.

### Step 2: Load Dataset
Load the Advertising dataset from CSV file.

### Step 3: Exploratory Data Analysis
- Display first few rows
- Check data types and missing values
- Generate statistical summaries
- Visualize feature distributions

### Step 4: Data Preprocessing
- Visualize distributions of features
- Create scatter plots to understand relationships
- Analyze correlation between TV spend and Sales

### Step 5: Feature Selection
- Select `TV` as the input feature (X)
- Select `Sales` as the target variable (y)

### Step 6: Train-Test Split
Split the data into training (80%) and testing (20%) sets.

### Step 7: Model Initialization
Initialize the Linear Regression model.

### Step 8: Model Training
Train the model using the training dataset to learn the relationship: **Y = mX + C**

### Step 9: Model Testing
Use the trained model to predict sales on the test set.

### Step 10: Model Evaluation
Evaluate model performance using:
- **Mean Absolute Error (MAE)**
- **R² Score (Coefficient of Determination)**

### Step 11: Extract Model Parameters
- **Slope (m):** Coefficient showing the relationship strength
- **Intercept (C):** Base sales value when TV spend is zero

### Step 12: Visualization
Plot the regression line along with actual data points to visualize model fit.

## 📈 Model Performance

The model is evaluated using:

- **Mean Absolute Error (MAE):** Measures average prediction error (~2.4 units)
- **R² Score:** Indicates how well the model explains variance in sales

**Regression Equation:** 
```
Sales = 0.0465 × TV + 7.1196
```

This equation means:
- For every $1,000 increase in TV advertising, sales increase by approximately 46.5 units
- When TV spend is $0, baseline sales are approximately 7,120 units

## 📊 Key Insights

- TV advertising shows a positive correlation with sales
- The linear relationship is captured effectively by the model
- The model provides reasonable predictions for sales based on TV spend
- R² score indicates the percentage of variance explained by the model

## 🔄 Future Enhancements

- [ ] Implement Multiple Linear Regression using all features (TV, Radio, Newspaper)
- [ ] Add cross-validation for more robust evaluation
- [ ] Implement polynomial regression for non-linear relationships
- [ ] Add feature engineering and interaction terms
- [ ] Deploy the model as a web application
- [ ] Add residual analysis and assumption checking
