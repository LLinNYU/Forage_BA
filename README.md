# The Forage: British Airways  
This project is one of the many job simulations available on Forage that allows students to experience what it's like working at certain companies.

## Table of Contents  
- [Overview](#Overview)
- [Structure](#Structure)

## Overview
The Forage: British Airways is a data science job simulation that involves web scraping, analyzing data, and creating a predictive model to answer realistic business questions such as "What topics are discussed in reviews for the service?" and "What are the factors considered in a customer's purchase?" for British Airways.  

This simulation introduced me to web scraping and handling natural language tasks. This was also good practice with binary classification models.

## Structure
- data - folder containing the notebooks that processed the data and the relevant csv files  
- Part_1_Data_Overview.ipynb - the python notenook containing analysis of the scraped reviews data and their sentiments about their experience with British Airways
- Part_2_Predictive_Model.ipynb - the python notebook containing the RandomForestClassifier model that predicts whether a customer decides to create a booking or not

## Installation
1. Clone the repository: 'git clone https://github.com/LLinNYU/Forage_BA.git'
2. Navigate to the dierctory: 'cd Forage_BA'
3. Install dependencies:
   pip install wordcloud


## Acknowledgements:  
Libraries used: numpy, sklearn, pandas, matplotlib, NLTK, wordcloud  
Other resources for learning: textblob, spacy, ChatGPT
