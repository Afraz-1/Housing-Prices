# California Housing Price Prediction

## Overview
This project predicts California housing prices using machine learning techniques. The model analyzes various features including geographical location, housing characteristics, and demographic data to estimate median house values.

## Dataset
- **Source**: California Housing Dataset
- **Features**: longitude, latitude, housing_median_age, total_rooms, total_bedrooms, population, households, median_income, ocean_proximity
- **Target**: median_house_value
- **Size**: 20,640 samples

## Project Structure
```
├── housing_analysis.ipynb    # Main Jupyter notebook with complete analysis
├── housing.csv              # Dataset
└── README.md               # Project documentation
```

## Key Features
- **Data Exploration**: Comprehensive EDA with visualizations and correlation analysis
- **Feature Engineering**: Created new features like rooms_per_household, bedrooms_per_room, population_per_household
- **Stratified Sampling**: Used income categories for proper train-test split
- **Preprocessing Pipeline**: Automated handling of numerical and categorical features
- **Model Comparison**: Linear Regression, Decision Tree, Random Forest
- **Hyperparameter Tuning**: RandomizedSearchCV for optimal model performance

## Technologies Used
- **Python Libraries**: pandas, numpy, matplotlib, scikit-learn
- **ML Algorithms**: Linear Regression, Decision Tree Regressor, Random Forest Regressor
- **Preprocessing**: StandardScaler, SimpleImputer, OneHotEncoder, ColumnTransformer
- **Model Selection**: Cross-validation, RandomizedSearchCV

## Results
- **Best Model**: Random Forest Regressor
- **Final RMSE**: ~47,000 (optimized through hyperparameter tuning)
- **Best Parameters**: Determined through randomized search across multiple hyperparameters

## How to Run
1. Clone the repository
2. Install required dependencies: `pip install pandas numpy matplotlib scikit-learn jupyter`
3. Open `housing_analysis.ipynb` in Jupyter Notebook
4. Run all cells sequentially

## Key Insights
- Median income shows the strongest correlation with house values
- Feature engineering improved model performance
- Random Forest outperformed linear models significantly
- Geographical features (longitude/latitude) are important predictors

## Future Improvements
- Implement ensemble methods
- Add more sophisticated feature engineering
- Try deep learning approaches
- Include external data sources (crime rates, school ratings, etc.)
