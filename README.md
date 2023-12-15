# ML_in_FRE_Project
This project researched on News's impact on Stock Market using Dow Jones Index as an indicator.
All analysis is conducted using google colab, showing as 'Team `Name Undecided`.ipynb' file in the repo.
Link for colab notebook: https://colab.research.google.com/drive/1BqWA0-XU5XQf07PYIwrEfV4-hq7wVQus?usp=drive_link
Link for Streamlit Dashoard App: https://mlinfreprojectapp-hfss9yse9q75tyt9rxuosb.streamlit.app/
## Research Procedure
* Data Loading and Basic EDA
* Sentiment Analysis
* Machine Learning Based on TF-IDF Vectorizer and Sentiments
* Time Series Analysis using SARIMAX Model
## Data Description
* DJIA data, Shape(1989,27): Dialy Dow Jones Industrial Average (DJIA)
* News data, Shape(1989,27): Historical news headlines from Reddit WorldNews Channel (/r/worldnews). They are ranked by reddit users' votes, and only the top 25 headlines are considered for a single date.
## Models
Two types of Machine Learning models are built, targeting on the 'label' variable with '0' representing DJIA decreasing and '1' representing DJIA increasing or stay the same.
* Model 1: Use text data as input, applied TF-IDF vectorizer and trained multiple models.
* Model 2: Use results of sentiment analysis as input (compound, polarity, subjectivity, pos, neg, and neu). Devide Top1-25 news to 3 groups: 1. Top1-8, 2. Top9-17, and 3. Top18-25. Trained models respectively on 3 groups and all 25 news.
* Evaluation Metrics: Accuracy, Precision, F-score, Recall, MAPE, RMSE and R square.
## Time Series Analysis
SARIMAX (Seasonal Autoregressive Moving Average) model is used to analyze DJIA data, and make forecasting.
## Application Demo
Streamlit Link: https://mlinfreprojectapp-hfss9yse9q75tyt9rxuosb.streamlit.app/

App Github Repo link: https://github.com/OliverHu726/ML_in_FRE_Project_App

We have built a streamlit app with two functions:
* Make predictions on the increase or decrease label of DJIA with user input
* Showing important analysis results of this project






