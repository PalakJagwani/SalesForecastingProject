# Sales Forecasting Project

## Overview

This project aims to predict future sales for a company based on historical sales data. It utilizes machine learning models to provide accurate forecasts, helping businesses make informed decisions regarding inventory management, resource allocation, and sales strategies.

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib 
- Seaborn
- Scikit-learn
- Jupyter Notebooks
- Facebook Prophet

## Data

The project uses historical sales data of different stores in Europe, which contains various features such as:
Input data :
- Id : Transaction Id (Combination of Store and data).
- Store : Unique Store id.
- Customers : Number of customers on a given day.
- Open : Boolean Value to indicate if store is open(1) or not (0).
- Promo : Describes if a store is running a promo on that day or not.
- StateHoliday : Indicates which type of state holiday is it : (a = public holiday, b = EasterHoliday, c = Chrishtmas, 0 = none).
- SchoolHoliday : Indicates if the store,date (Transaction) was affected by a school holiday.
- StoreType : Categorical data to indicate type of store(a, b, c, d).
- Assortment : a = basic, b = extra, c = extended.
- CompetitionDistance(meters) : Distance to Competitor store.
- CompetitorOpenSincemonth [Month/Year] : Date when competion was open.
- Promo2 : Continuing and consecutive promotion for some store (0 : Store is not participating, 1 : Store is participating).
- Promo2Since [Year/Month] : Date when store started participating in Promo2.
- PromoInterval : Describes the consecutive intervals Promo2 is started, naming the months promotion is started from(Duration Promo2 has been running for).

Output Data :
- Sales (in Euros) : sales / day


## Steps Involved

1. **Data Preprocessing**: The data is cleaned and prepared for modeling, including handling missing values.
2. **Exploratory Data Analysis (EDA)**: Various visualizations and analyses are performed to identify patterns and correlations in the data.
3. **Modeling**: The Facebook Prophet Model is used for Time Series Analysis in order to perform Sales Forecasting.

## Installation

1. Clone this repository:

   ```
   git clone https://github.com/PalakJagwani/MovieReviewSentimentAnalysis.git
   ```

2. Install the required dependencies:

```
pip install -r requirements.txt
```