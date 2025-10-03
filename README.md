# hotel_reviews_analysis
Analysis of European hotel reviews (Kaggle dataset). Data cleaning, exploratory analysis, and insights on customer satisfaction.

# DataHotel — Customer Reviews Analysis

## About
This project analyzes hotel reviews in Europe (Kaggle dataset, 2015–2017).  
The objective is to identify the main factors influencing customer satisfaction and provide actionable insights.

## Dataset
- Source: [Booking.com reviews collected via Kaggle](https://www.kaggle.com/datasets/michelhatab/hotel-reviews-bookingcom)  
- Size: 515,739 reviews (238 MB)  
- Columns: hotel address, nationality, review date, average score, stay tags, etc.  
- For demonstration purposes, this repository uses a **20,000-row sample** stored in `data/hotel_reviews_sample.csv`.  
- The sample was created from the full dataset to keep the notebook lightweight and executable directly on Google Colab.  
- The complete dataset can be downloaded from Kaggle.

## Methodology
1. Data cleaning (handling missing values, duplicates, tag normalization)  
2. Exploratory Data Analysis (EDA)  
3. Classification of stay tags (trip type, traveler type, room type, etc.)  
4. Visualization of satisfaction patterns (by country, season, traveler profile)

## Results
- Seasonal patterns in satisfaction  
- Differences by traveler type and nationality  
- Impact of room type on reviews  
- Influence of the number of reviews posted by a user on the severity of their ratings

## Tools
- Python  
- Libraries: `numpy`, `pandas`, `matplotlib`, `seaborn`, `scipy`, `statsmodels`  
- Google Colab

## How to use
- Open the notebook: `hotel_reviews_analysis.ipynb`  
- The notebook automatically loads the sample dataset from GitHub:  
  ```python
  import pandas as pd
  
  url = "https://raw.githubusercontent.com/marionortega/hotel_reviews_analysis/refs/heads/main/data/hotel_reviews_sample.csv"
  df = pd.read_csv(url)
  df.head()
