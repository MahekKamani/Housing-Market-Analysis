# Housing Market Analysis

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-1.x-orange.svg)
![Seaborn](https://img.shields.io/badge/Seaborn-0.11.x-green.svg)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.x-red.svg)

## Overview

The **Housing Market Analysis** project is a comprehensive data analysis and visualization initiative aimed at uncovering insights from housing market data. This project leverages Python and popular data science libraries to explore, clean, and analyze housing data, providing actionable insights into factors influencing housing prices.

## Features

- **Data Cleaning**: Handle missing values, duplicates, and outliers.
- **Exploratory Data Analysis (EDA)**: 
  - Statistical summaries of key features.
  - Visualizations such as histograms, scatter plots, and box plots.
- **Feature Analysis**:
  - Correlation analysis between features and sale prices.
  - Neighborhood-wise price distribution.
- **Visualizations**:
  - Distribution of housing prices.
  - Relationships between features like `GarageArea`, `GrLivArea`, and `SalePrice`.
  - Count plots for categorical variables like `OverallQual` and `MSZoning`.

## Dataset

The dataset used in this project contains 81 features and 1460 entries, including details about property characteristics, sale conditions, and prices.

### Key Features:
- **SalePrice**: The target variable representing the sale price of the property.
- **GrLivArea**: Above-ground living area in square feet.
- **OverallQual**: Overall material and finish quality.
- **YearBuilt**: Original construction date.
- **GarageArea**: Size of the garage in square feet.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/MahekKamani/Housing-Market-Analysis.git
   cd Housing-Market-Analysis
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook Housing_Data_Analytics.ipynb
   ```

## Usage

1. **Load the Dataset**: The dataset is loaded using Pandas.
2. **Run the Notebook**: Execute the cells in the `Housing_Data_Analytics.ipynb` file to perform data cleaning, analysis, and visualization.
3. **Explore Visualizations**: Use the generated plots to gain insights into the housing market.

## Visualizations

### 1. Sale Price Distribution
![Sale Price Distribution](https://github.com/MahekKamani/Housing-Market-Analysis/blob/main/images/pricevssize.png)

### 2. Sale Price vs Overall Quality
![Sale Price vs Overall Quality](https://github.com/MahekKamani/Housing-Market-Analysis/blob/main/images/yearbuiltvsprice.png)

### 3. Neighborhood-wise Average Sale Price
![Neighborhood-wise Average Sale Price](https://github.com/MahekKamani/Housing-Market-Analysis/blob/main/images/heatmap.png)

## Key Insights

1. **Neighborhood Impact on Sale Prices**:
   - Properties located in certain neighborhoods, such as `StoneBr` and `NridgHt`, consistently show higher average sale prices compared to others like `MeadowV` and `IDOTRR`.
   - This indicates that location is a significant factor influencing property values, likely due to factors such as school districts, amenities, and overall desirability.

2. **Feature Correlation with Sale Price**:
   - **GrLivArea (Above Ground Living Area)**: Strong positive correlation with `SalePrice` (correlation coefficient ~0.7). Larger homes tend to sell for higher prices.
   - **OverallQual (Overall Quality)**: One of the strongest predictors of `SalePrice`. Higher quality materials and finishes significantly increase property value.
   - **GarageArea**: Moderate positive correlation with `SalePrice`. Larger garages add value but not as strongly as living area or quality.

3. **Year Built and Renovation Trends**:
   - Homes built or renovated more recently tend to have higher sale prices, reflecting modern construction standards and updated features.
   - Properties built before 1950 generally have lower sale prices unless they have undergone significant renovations.

4. **Distribution of Sale Prices**:
   - The distribution of sale prices is right-skewed, with most properties priced below $200,000.
   - High-value properties (above $500,000) are rare and often located in premium neighborhoods or have unique features.

5. **Impact of Categorical Variables**:
   - **MSZoning (Zoning Classification)**: Residential zones (`RL` and `RM`) dominate the dataset, with `RL` properties generally commanding higher prices.
   - **OverallCond (Overall Condition)**: While less impactful than `OverallQual`, properties with better overall condition tend to sell for slightly higher prices.

6. **Outliers and Anomalies**:
   - A few properties with extremely high sale prices (above $700,000) were identified as outliers. These are likely luxury homes with unique features.
   - Some properties with large living areas but low sale prices suggest potential data entry errors or distressed sales.

7. **Neighborhood-Specific Trends**:
   - Certain neighborhoods exhibit a wider range of sale prices, indicating diverse property types and conditions.
   - Neighborhoods like `OldTown` and `Edwards` show more affordable housing options, while `NoRidge` and `Veenker` cater to higher-income buyers.

8. **Lot Area and Sale Price**:
   - While larger lot areas generally correlate with higher sale prices, the relationship is weaker compared to living area or quality. This suggests that buyers prioritize usable living space over lot size.

9. **Seasonality in Sales**:
   - Properties sold during spring and summer months tend to have slightly higher sale prices, likely due to increased buyer activity during these seasons.

10. **Key Takeaways for Stakeholders**:
    - **Homebuyers**: Focus on properties in neighborhoods with strong appreciation trends and prioritize features like living area and quality.
    - **Sellers**: Renovating key areas (e.g., kitchens, bathrooms) and improving overall quality can significantly boost sale prices.
    - **Investors**: Target undervalued neighborhoods with potential for growth, and consider properties with strong correlation features like `GrLivArea` and `OverallQual`.

---

These insights provide a comprehensive understanding of the factors influencing housing prices and can guide decision-making for buyers, sellers, and investors.

## Technologies Used

- **Python**: Core programming language.
- **Pandas**: Data manipulation and analysis.
- **NumPy**: Numerical computations.
- **Matplotlib & Seaborn**: Data visualization.

## Project Structure

```
Housing-Market-Analysis/
├── Housing_Data_Analytics.ipynb  # Main Jupyter Notebook for analysis
├── train.csv                     # Dataset file
├── requirements.txt              # Python dependencies
└── README.md                     # Project documentation
```

---

Thank you for exploring the **Housing Market Analysis** project! 🚀
