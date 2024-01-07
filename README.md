# The Forage: British Airways  
This project is one of the many job simulations available on Forage that allows students to experience what it's like working at certain companies.

## Table of Contents  
- [Overview](#Overview)
- [Structure](#Structure)
- [Installation](#Installation)
- [Acknowledgements](#Acknowledgements)

## Overview
The Forage: British Airways is a data science job simulation that involves web scraping, analyzing data, and creating a predictive model to answer realistic business questions such as "What topics are discussed in reviews for the service?" and "What are the factors considered in a customer's purchase?" for British Airways.  

This simulation provides an introduction to web scraping, handling natural language tasks, and binary classification models.  
The reviews are scraped from Skytrax's review site: https://www.airlinequality.com/ .  
Part 1 focuses on isolating the verified reviews from the site, creating histograms for the basic statistics of the data, creating a wordcloud, forming n-grams for the reviews, and gauging customer's opinions on the services.  
Part 2 uses RandomForestClassifier with the default parameters (uses gini criterion, no tree depth limit, 100 trees) and 5 folds for cross validation. The accuracy was about 0.85, recall was about 0.13, precision was about 0.50, F1 score was about 0.20, and AUC was about 0.77. Since there are significantly fewer confirmed bookings, this model is quite weak in predicting confirmed bookings. About half of the predicted bookings are true bookings. However, this model appears to have performed better than the model answer by accuracy and recall, perhaps due to more data in recent years. Furthermore, top features were considered to be less influential than in the model answer, although the features were still consistent.  

## Structure
- data: folder containing the notebooks that processed the data and the relevant csv files  
- Part_1_Data_Overview.ipynb: the python notenook containing analysis of the scraped reviews data and their sentiments about their experience with British Airways
- Part_2_Predictive_Model.ipynb: the python notebook containing the RandomForestClassifier model that predicts whether a customer decides to create a booking or not

## Installation
1. Clone the repository: ```git clone https://github.com/LLinNYU/Forage_BA.git```
2. Navigate to the dierctory: ```cd Forage_BA```
3. Install dependencies:  
   ```pip install wordcloud nltk```  
   ```nltk.download('punkt')```  
   ```nltk.download('stopwords')```  

## Acknowledgements:  
Libraries used: numpy, sklearn, pandas, matplotlib, NLTK, wordcloud  
Other resources for learning: textblob, spacy, ChatGPT
