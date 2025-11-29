# Real-Estate-Analysis

🏠 Mumbai Rental Market Analysis & Rent Price Prediction

This repository contains the complete code and analysis for a deep dive into the Mumbai housing rental market. This project was executed from the perspective of a Data Analyst advising a real estate investment firm (like SP Property Solutions) on strategic pricing, investment, and client advisory.


🌟 Executive Summary

The analysis successfully built a Random Forest Regression Model that explains 78% of the variance in rent ($R^2=0.7798$) and has an average prediction error of $\mathbf{INR\ 20,945}$ (MAE). The key finding is that while property size is the largest determinant of rent, location, and the number of bathrooms are critical factors for achieving premium rental yields.


💡 Key Business Insights

| Area | Finding | Actionable Insights |
| --- | --- | --- |
| Pricing Model | $R^2$ Score of $\mathbf{0.7798}$ with an MAE of $\mathbf{\text{INR}\ 20,945}$. | Forecasting Tool: The model is highly accurate and can be integrated into the sales process to provide immediate, data-backed rental quotes to property owners, giving the company a competitive advantage. |
| Rent Drivers | House Size ($\mathbf{\text{sqft}}$) accounts for $\approx 66\%$ of the predictive power, followed by Number of Bathrooms ($\approx 11\%$). | Client Advisory: When advising owners on renovations, prioritize increasing the number of bathrooms (where possible), as the model shows this has a strong, quantifiable impact on rental price. |
| Market Segment | The median rent is $\mathbf{\text{INR}\ 40,000}$, but high-end properties in clusters like Jacob Circle (Avg. Rent $\text{INR}\ 950,000$) skew the market. | Investment Strategy: Prioritize investment and development in the top 10 premium zones to maximize rental yield and capital appreciation. |


🛠️ Methodology & Technology

Key Steps

Data Cleaning: Handled missing values (imputing 0 for missing amenity counts) and converted string-based features (house_size) to numerical.

Feature Engineering: Created the key metric price_per_sqft (Rental Efficiency) for comparative market analysis.

Geospatial Analysis: Used Latitude and Longitude to visualize rental efficiency across Mumbai.

Modeling: Used One-Hot Encoding (grouping low-frequency locations as 'Other') and trained a Random Forest Regressor.

Technology Stack

Language: Python

Data Manipulation: pandas, numpy

Visualization: matplotlib, seaborn

Machine Learning: scikit-learn (Random Forest Regressor)


📈 Visual Results

1. Top Feature Importances

This plot quantifies the direct impact of each feature on the monthly rental price.

2. Geospatial Rental Efficiency Map

This scatter plot maps all properties using latitude and longitude. The color and size of the points represent the Rent per Square Foot, clearly showing the high-efficiency rental clusters in South Mumbai.

3. Top 10 Most Expensive Rental Locations

The locations commanding the highest average rent.



⚙️ How to Run the Project Locally

To replicate this analysis, ensure you have the required libraries installed and follow these steps:

Clone the Repository:

git clone [YOUR_REPOSITORY_URL]


Install Dependencies:

pip install pandas numpy matplotlib seaborn scikit-learn


Data File: Place the data file (Indian_housing_Mumbai_data.csv) into the root directory of the project folder.

Execute the Script:

python mumbai_rental_analysis.py
(Note: Replace mumbai_rental_analysis.py with your Python file name.)

