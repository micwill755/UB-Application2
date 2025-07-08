# Used Car Price Analysis: Final Report

## Project Overview

This project analyzes a large dataset of used cars to identify which factors most strongly influence vehicle pricing. The insights from this analysis will help used car dealers better prioritize inventory selection and pricing strategies.

## Objective

Our objective was to analyze a comprehensive used car dataset to identify the key factors that drive vehicle pricing, enabling dealers to make data-driven decisions about inventory management and pricing strategies.

## Data Preparation & Methodology

We cleaned and prepared the dataset through several key steps:

- **Data Cleaning**: Removed duplicate and invalid VINs
- **Feature Engineering**: Created new features such as vehicle age
- **Missing Value Handling**: Replaced unknown conditions and handled missing data
- **Categorical Encoding**: Applied one-hot encoding to categorical variables
- **Feature Scaling**: Normalized numerical features (odometer readings, cylinders, etc.)

## Model Performance

We trained and evaluated several regression models:
- Linear Regression
- Ridge Regression  
- Lasso Regression

### Best Model Results

The **Linear Regression model with preprocessing** achieved the best performance:

- **Test RMSE: $5,191.95**
- **Test MAE: $3,571.45**

These metrics indicate that on average, our model's predictions are within approximately **$3.5K–$5.1K** of the actual price, representing a significant improvement over baseline models.

## Key Insights: Top Features Driving Price

Our analysis revealed the top 10 vehicle features that have the strongest impact on pricing:

### High-Value Models Include:
- **Hummer H1** - Premium off-road vehicle
- **Freightliner Service Trucks** - Commercial utility vehicles
- **Freightliner Dump Trucks** - Heavy-duty commercial vehicles
- **BMW E39 M5** - High-performance luxury sedan

These models show coefficients in the range of **$40K–$52K**, indicating they are strong drivers of higher vehicle prices.

### Key Factors:
- **Vehicle Model**: Specific models have dramatic impact on pricing
- **Fuel Type**: Alternative fuel types can significantly affect value
- **Vehicle Condition**: Condition ratings are major price contributors
- **Specialty/Commercial Vehicles**: Often command premium prices

## Business Recommendations

Based on our analysis, we recommend the following strategies for used car dealers:

### 1. **Focus Inventory on High-Value Models**
- Prioritize acquisition of models like Hummer H1 and Freightliner trucks
- These consistently drive higher prices and may yield better returns
- Consider the specialty vehicle market for premium opportunities

### 2. **Maintain and Highlight Vehicle Condition**
- Vehicles marked as "excellent" or "like new" are strong price indicators
- Invest in vehicle preparation and reconditioning
- Emphasize condition ratings in marketing and listings

### 3. **Explore Niche Segments**
- Specialty and commercial vehicles command significantly higher prices
- Consider expanding into these less common but profitable segments
- Build expertise in evaluating and marketing specialty vehicles

### 4. **Implement Data-Driven Pricing Strategy**
- Use model predictions to guide pricing decisions
- Regularly update pricing based on market conditions
- Leverage feature importance for inventory acquisition decisions

## Technical Implementation

The analysis was implemented using:
- **Python** for data processing and modeling
- **Scikit-learn** for machine learning models and preprocessing
- **Pandas** for data manipulation
- **Matplotlib/Seaborn** for visualization
- **Jupyter Notebooks** for analysis workflow

## Model Features

The final model incorporates:
- **Numerical Features**: Odometer reading, cylinders, age
- **Categorical Features**: Make, model, fuel type, transmission, condition, etc.
- **Preprocessing Pipeline**: Scaling for numerical features, one-hot encoding for categories

## Next Steps

1. **Deploy Model Dashboard**: Create a simple interface for real-time price predictions
2. **Continuous Model Updates**: Regularly retrain with new market data
3. **Expand Feature Set**: Incorporate additional market indicators
4. **A/B Testing**: Test pricing strategies based on model recommendations
5. **Regional Analysis**: Adapt model for different geographic markets

## Files in This Repository

- `prompt_II.ipynb` - Complete analysis notebook with data exploration, modeling, and results
- `README.md` - This summary report
- `data/` - Dataset files (if included)
- `requirements.txt` - Python dependencies

## Conclusion

This analysis demonstrates that machine learning can provide valuable insights for used car pricing. With a prediction accuracy within $3.5K-$5.1K, dealers can make more informed decisions about inventory acquisition and pricing strategies. The identification of high-value models and key pricing factors provides actionable intelligence for improving profitability in the used car market.

The model's ability to identify specialty vehicles and commercial trucks as premium segments opens new opportunities for dealers willing to expand beyond traditional passenger vehicles.
