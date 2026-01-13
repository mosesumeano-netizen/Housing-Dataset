# Housing Price Analysis (Excel-Based)

![Image](https://github.com/user-attachments/assets/aee5cb62-afbe-45f5-9e28-6afc4ba09721)

This project analyzes factors that influence housing prices using Microsoft Excel. Statistical techniques such as 
descriptive statistics, correlation analysis, and multiple regression were applied.

## Dataset Overview

Source: Kaggle Housing Dataset

Rows: 546

Columns: 13

Target Variable: Price

## Key Variables

Numerical: Area, Bedrooms, Bathrooms, Stories, Parking

Categorical (Yes/No):
MainRoad, GuestRoom, Basement, Hot Water Heating,
AirConditioning, Preferred Area, Furnishing Status

##  Data Preparation in Excel
Convert Yes/No to Binary (1/0)

Excel formula used:

=IF(A2="Yes",1,0)


This conversion allows categorical variables to be used in:

Correlation analysis

Regression modeling

##  Descriptive Statistics

Excel functions used:

=AVERAGE(range)
=MIN(range)
=MAX(range)
=STDEV.P(range)

Summary Highlights

Average house price ≈ 4.77 million

Average land size ≈ 5,151 sq ft

Most houses have 3 bedrooms, 1–2 bathrooms, and 2 stories

##  Correlation Analysis

Excel formula:

=CORREL(price_range, variable_range)

Binary Variables vs Price
Variable	Correlation
Air Conditioning	0.453
Preferred Area	0.330
Main Road	0.297
Guest Room	0.256
Basement	0.187
Hot Water Heating	0.093

Insight: Comfort and location-related features show stronger relationships with house price.

Numerical Variables vs Price
Variable	Correlation
Area (sq ft)	0.536
Bathrooms	0.518
Stories	0.421
Parking	0.384
Bedrooms	0.366

Insight: Property size and number of bathrooms influence price more than bedroom count.

##  Multiple Regression Analysis

Regression was performed using:

Data → Data Analysis → Regression

Model Statistics

R²: 0.682

Adjusted R²: 0.674

F-statistic: 87.52

Significance F: 9.07E-123

The model explains 68% of the variation in housing prices.

Significant Predictors (p < 0.05)
Variable	Impact on Price
Area (sq ft)	+244 per sq ft
Bathrooms	+987,668
Air Conditioning	+864,958
Hot Water Heating	+855,447
Preferred Area	+651,544
Stories	+450,848
Fully Furnished	+411,234
Parking	+277,107
Not Significant

Bedrooms (p = 0.114)
→ Not a strong predictor when other variables are considered.
 Likely due to area of rooms and living spaces not given in the dataset
## Key Findings

House prices are driven mainly by land size, bathrooms, location, and amenities

Binary variables, when properly encoded, add meaningful insights

Excel is sufficient for robust housing price analysis

##  Tools Used

Microsoft Excel (Data Cleaning, Correlation, Regression)

Power BI (Visualization – optional)

GitHub (Project Documentation)

##  Conclusion

This project demonstrates how Excel-based statistical analysis can effectively identify the key drivers of
housing prices, making it suitable for academic work and data analytics portfolios.

##  Recommendation

Dataset to include details about size of houses, not just land size. The area of rooms available for internal
living spaces, and other external variables to include cost of financing. Location of land to be categoried
as to compare land in choice area and the houses there




