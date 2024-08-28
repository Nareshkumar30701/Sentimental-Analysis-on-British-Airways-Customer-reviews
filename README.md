# British Airways Review Analysis
## Project Overview
This project aims to analyze customer reviews of British Airways using Natural Language Processing (NLP) techniques. The analysis involves web scraping reviews, cleaning and preprocessing the text data, identifying latent topics using Latent Dirichlet Allocation (LDA), and performing sentiment analysis on the reviews. The insights gained are then visualized using word clouds and sentiment distribution plots.

## Features
Web Scraping: Reviews are scraped from the British Airways review pages on the AirlineQuality website.
Text Preprocessing: The raw text data is cleaned by removing special characters, stopwords, and lemmatizing the words.
Topic Modeling: LDA is used to identify underlying topics within the reviews.
Word Clouds: Word clouds are generated for each topic to visualize the most prominent words.
Sentiment Analysis: Each review is classified as either Positive or Negative based on the sentiment polarity.
Sentiment Distribution: Sentiment distribution is visualized for all reviews and broken down by topic.
## Dataset
The data is scraped from the British Airways review pages available on AirlineQuality. The script extracts at least 100 reviews for analysis.

## Usage
Run the script:

Execute the script in a Jupyter Notebook or Colab to scrape the reviews, process the text, and generate analysis.
The script is self-contained and performs the entire workflow from data extraction to visualization.
Customize the analysis:

Modify the num_topics variable to adjust the number of topics extracted by the LDA model.

## Key Components
Web Scraping:

The get_reviews_from_page and get_100_reviews functions scrape reviews from the specified URL.
Text Preprocessing:

The clean_text function handles text cleaning, including removing stopwords, tokenization, and lemmatization.
Topic Modeling:

LDA is used to extract topics from the reviews, and the top words for each topic are displayed.
Sentiment Analysis:

The analyze_sentiment function classifies the sentiment of each review.
Sentiment distribution is plotted for a general overview and for each identified topic.
Visualization:
Word clouds are generated for each topic to visualize important words.
Sentiment distributions are plotted to understand customer sentiment across topics.


## Results
The LDA model successfully identifies major topics in the customer reviews.
Sentiment analysis provides insights into the overall sentiment of customers toward British Airways, and how this sentiment varies across different topics.
Requirements
Python 3.x
Required Python packages (as per requirements.txt):
beautifulsoup4
requests
pandas
nltk
scikit-learn
matplotlib
wordcloud
textblob

## Conclusion
This project demonstrates how to combine web scraping, NLP, and machine learning techniques to derive insights from customer reviews. The ability to understand customer sentiment and identify key topics provides valuable information that can help improve customer service and address common issues.

## Future Work
Increase the number of reviews: Scraping more reviews could lead to more accurate topic modeling and sentiment analysis.
Fine-tune LDA model parameters: Experimenting with different numbers of topics and other LDA hyperparameters could yield better insights.
Incorporate additional analysis: Include more advanced sentiment analysis techniques or other forms of textual analysis like aspect-based sentiment analysis.
