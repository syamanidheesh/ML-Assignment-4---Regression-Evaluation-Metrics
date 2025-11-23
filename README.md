# Regression Analysis on California Housing Dataset

A comprehensive machine learning workflow for regression analysis on the California Housing dataset, covering the complete data science pipeline from data loading and preprocessing to model implementation, hyperparameter tuning, and performance evaluation.

## 📊 Dataset Information

**Source:** `sklearn.datasets.fetch_california_housing`

- **Samples:** 20,640
- **Features:** 8 numeric predictive attributes
- **Target:** Median house value for California districts (expressed in hundreds of thousands of dollars)

### Feature Description

| Feature | Description |
|---------|-------------|
| MedInc | Median income in block group |
| HouseAge | Median house age in block group |
| AveRooms | Average number of rooms per household |
| AveBedrms | Average number of bedrooms per household |
| Population | Block group population |
| AveOccup | Average number of household members |
| Latitude | Block group latitude |
| Longitude | Block group longitude |

## 🏗️ Project Structure

### 1. Data Loading and Preprocessing
- Loaded California Housing dataset from sklearn
- Converted data to pandas DataFrame for easier manipulation
- Added target column 'MedHouseVal' to the dataset

### 2. Exploratory Data Analysis (EDA) and Data Cleaning
- Dataset shape and basic information analysis
- Statistical summary using `describe()` method
- Missing values and duplicate detection
- Outlier detection and handling using Inter Quartile Range (IQR) method
- Data distribution analysis through histograms
- Feature correlation analysis using heatmaps

### 3. Model Implementation
Implemented and evaluated three regression models:
- **Linear Regression**
- **Decision Tree Regressor**
- **Random Forest Regressor**

### 4. Model Evaluation Metrics
Comprehensive evaluation using:
- **Mean Absolute Error (MAE)**
- **Mean Squared Error (MSE)**
- **R-squared Score (R²)**

### 5. Hyperparameter Tuning
- **GridSearchCV** for systematic parameter optimization
- Cross-validation for robust performance assessment
- Significant performance improvement observed after tuning

## 🔍 Key Findings

### Model Performance Summary

#### Linear Regression
- Works reasonably well as a baseline model
- Limited by non-linear relationships in the data
- Cannot capture complex patterns in housing data effectively

#### Decision Tree Regressor
- Good initial performance
- Prone to overfitting without proper regularization
- Performance improves significantly with hyperparameter tuning

#### Random Forest Regressor
- **Best overall performance**
- Handles non-linear relationships effectively
- Reduces overfitting through ensemble methods
- Most stable and reliable predictions
- Highest and most consistent R² scores

## 🛠️ Technical Implementation

### Libraries Used
- `scikit-learn`
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`

### Key Techniques
- **Preprocessing:** StandardScaler for feature scaling
- **Model Selection:** Multiple algorithms with comparative analysis
- **Validation:** Train-test split and cross-validation techniques
- **Optimization:** GridSearchCV for hyperparameter tuning

## 📈 Results

The Random Forest Regressor emerged as the superior model for this regression task, demonstrating robust performance in predicting California housing prices. The ensemble approach effectively handled the complex, non-linear relationships in the dataset, while hyperparameter tuning proved crucial for optimizing model performance across all algorithms.

## 🎯 Conclusion

This project showcases a complete machine learning workflow suitable for regression problems, with emphasis on proper evaluation methodologies and model optimization techniques. The implementation demonstrates best practices in data preprocessing, model selection, and performance evaluation that can be applied to similar regression tasks.


