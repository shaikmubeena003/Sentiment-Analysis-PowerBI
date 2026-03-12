# Sentiment-Analysis-PowerBI

# Twitter Brand Sentiment Monitoring using Python, SQL, and Power BI

## 1. Project Overview

Social media platforms like Twitter contain large amounts of user
opinions about brands, products, and services. Organizations can analyze
this data to understand customer perception.

This project focuses on analyzing Twitter data to determine whether
tweets express **positive or negative sentiment**. The data is processed
using **Python**, stored in a **SQLite database**, and visualized using
**Power BI dashboards**.

The goal of this project is to demonstrate a **complete data analytics
pipeline** from data collection to business insights.

------------------------------------------------------------------------

## 2. Project Objectives

• Collect and analyze Twitter sentiment data\
• Clean and preprocess raw tweet data using Python\
• Store structured data in a SQL database\
• Implement a Star Schema data model for analysis\
• Build an interactive dashboard using Power BI\
• Visualize sentiment trends and insights

------------------------------------------------------------------------

## 3. Technologies Used

  Technology   Purpose
  ------------ -------------------------------------
  Python       Data cleaning and preprocessing
  Pandas       Data manipulation
  SQLite       Database storage
  Power BI     Data visualization
  GitHub       Project version control and hosting

------------------------------------------------------------------------

## 4. Dataset

Dataset Source: Kaggle

The dataset contains Twitter posts labeled with sentiment categories
such as **positive** and **negative**.

### Dataset Fields

  Column      Description
  ----------- -------------------------
  id          Unique tweet identifier
  sentiment   Sentiment label
  tweet       Text of the tweet

Example:

  id   sentiment   tweet
  ---- ----------- ---------------------
  1    Positive    I love this product
  2    Negative    Very bad service

------------------------------------------------------------------------

## 5. Project Architecture

Dataset (Kaggle)\
↓\
Python Data Cleaning\
↓\
Processed Dataset\
↓\
SQLite Database\
↓\
Power BI Data Modeling\
↓\
Interactive Dashboard

------------------------------------------------------------------------

## 6. Data Preprocessing (Python)

Python was used to clean and prepare the dataset before analysis.

Steps performed:

1.  Import dataset using Pandas\
2.  Remove unnecessary columns\
3.  Rename tweet column to `clean_tweet`\
4.  Handle missing values\
5.  Export cleaned dataset\
6.  Store cleaned data in SQLite database

Libraries used:

-   pandas\
-   sqlite3

------------------------------------------------------------------------

## 7. Database Implementation

The cleaned dataset is stored in a **SQLite database**.

Database Name:

twitter_sentiment.db

Main Table:

clean_twitter_data

Table Structure:

  Column        Description
  ------------- ----------------------
  TweetID       Unique tweet ID
  clean_tweet   Processed tweet text
  Sentiment     Sentiment label

------------------------------------------------------------------------

## 8. Data Modeling in Power BI

The project implements a **Star Schema** data model.

### Fact Table

clean_twitter_data

  Column
  -------------
  TweetID
  clean_tweet
  SentimentID

### Dimension Table

Dim_Sentiment

  Column
  -------------
  SentimentID
  Sentiment

Relationship:

Dim_Sentiment (1) → clean_twitter_data (Many)

------------------------------------------------------------------------

## 9. Power BI Dashboard

An interactive dashboard was created to visualize sentiment insights.

Features:

• Sentiment distribution visualization\
• Tweet analysis insights\
• Interactive filtering and exploration

Visualizations used:

• Bar chart for sentiment distribution\
• Data table for tweet records\
• Interactive slicers for filtering

------------------------------------------------------------------------

## 10. Project Folder Structure

Sentiment-Analysis-PowerBI

data/\
│\
├── raw/\
│ └── twitter.csv\
│\
└── processed/\
└── clean_twitter_data.csv

database/\
└── twitter_sentiment.db

notebooks/\
└── twitter_analysis.py

dashboard/\
└── Twitter_Sentiment_Dashboard.pbix

README.md

------------------------------------------------------------------------

## 11. Key Insights

• Distribution of positive vs negative tweets\
• Overall sentiment trend toward the brand\
• Insights into customer opinions from social media

------------------------------------------------------------------------

## 12. Conclusion

This project demonstrates how raw social media data can be transformed
into meaningful insights using a modern data analytics pipeline.

The workflow integrates:

Python for data processing\
SQL for structured storage\
Power BI for interactive visualization

------------------------------------------------------------------------

## 13. Future Improvements

• Real-time Twitter API data collection\
• Machine learning sentiment classification\
• Advanced NLP analysis\
• Real-time Power BI dashboards

------------------------------------------------------------------------

## 14. Author

Shaik Mubeena\
Data Analytics / Power BI Project
