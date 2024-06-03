# Yelp Review Sentiment Analysis

This repository contains a Jupyter notebook created in Google Colab that demonstrates the use of Natural Language Processing (NLP) to perform sentiment analysis on Yelp reviews. The project leverages the TextBlob library to analyze and classify sentiments as positive, negative, or neutral.

## Introduction

Sentiment analysis is a method used in NLP to identify emotional tone behind words. This is especially useful for understanding customer opinions in text data like reviews, social media comments, etc. The TextBlob library simplifies text processing by providing an easy-to-use interface for common NLP tasks including sentiment analysis.

## Project Objective

The goal of this project is to utilize TextBlob's sentiment analysis capabilities on a set of random Yelp reviews to assess customer satisfaction and derive actionable insights from unstructured feedback data.

## Pre-requisites

To run this project you will need:

- A Google account to access Google Colab.
- Basic knowledge of Python and familiarity with Pandas and Matplotlib libraries.
- An understanding of basic NLP concepts.

## Libraries Used

- `TextBlob`: To perform sentiment analysis.
- `Pandas`: For data manipulation.
- `NumPy`: For numerical operations.
- `Scikit-learn`: For machine learning.
  
These can be installed through pip if not already available:

```shell
pip install textblob pandas numpy matplotlib seaborn
```

Make sure you also have the latest version of Jupyter if running locally:

```shell
pip install jupyter
```

## Dataset Information

The dataset used consists of randomly selected Yelp reviews. Each review has two main components: review_text (the actual content) and stars given by the reviewer which represent the rating (1 star being lowest, 5 stars being highest).

**Note:** You will need your own dataset file in CSV or JSON format that includes at least one column with textual reviews.

## Files Included 

- `Yelp_Reviews_Sentiment_Analysis.ipynb` - Main Jupyter notebook containing code for loading data, preprocessing text, analyzing sentiments using TextBlob and visualizing results.

## Steps To Follow
 
1. **Data Loading & Preprocessing**
   - Importing necessary libraries 
   - Loading review dataset
   - Cleaning texts (removing punctuations/stopwords)
   - Tokenization
2. **Term Frequency-Inverse Document Frequency (TF-IDF)**
   - Compute the "relative frequency" that a word appears in a document compared to its frequency across all documents in the corpus
   - More useful than "term frequency" for identifying "important" words in each document (high frequency in that document, low frequency in other documents)
   - Useful for search engine relevance scoring, text summarization, document clustering, and classification
   - Use to summarize random Yelp reviews

3. **Sentiment Analysis with TextBlob**
   - Calculating polarity and subjectivity scores using TextBlob 
   
4. **Insights Gathering**
    - Drawing conclusions based on analytics performed
    
5. **Conclusions**
   - Key takeaways from our sentiment analysis include:
     1. **High Accuracy**: Our model demonstrated high accuracy in classifying sentiments into positive, negative, and neutral categories. This suggests that the features extracted during the NLP process were effective in capturing the nuances of human emotion embedded within the text.
     2. **Model Robustness**: Throughout various parameter tuning and cross-validation steps, our model maintained strong performance metrics across different subsets of data which attests to its robustness.
     3. **Scalability**: The approach used can be scaled accommodate larger datasets or can be adapted to other domains beyond Yelp reviews with minimal adjustments making it versatile for broad applications.
     4. **Actionable Insights**: By identifying patterns in customer sentiments over time or across different service categories, businesses can derive actionable insights that inform strategic decisions such as improving product offerings or addressing specific concerns raised by customers.
     5. **Limitations & Areas for Improvement**: Despite achieving high accuracy levels, there remains some room for improvement particularly in distinguishing between sarcasm or contextually nuanced phrases. Further refinement could incorporate additional linguistic features or leverage more complex models such as deep learning algorithms to enhance understanding of subtle emotional cues.
     6. **Business Impact**: Implementing this model as part of a continuous feedback loop system can significantly impact how businesses respond to customer needs and maintain their competitive edge by being responsive to market sentiment. Automated sentiment analysis serves as an efficient tool saving valuable resources that would otherwise be spent on manual review processes providing real-time insights into consumer behavior trends.
     
---

Before running any cells ensure all dependencies mentioned above are installed within your environment.

For any questions or further assistance feel free to reach out through issues on this repository.
