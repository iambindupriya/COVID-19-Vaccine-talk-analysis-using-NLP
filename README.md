# COVID-19-Vaccine-talk-analysis-using-NLP
"Understanding people's sentiment, trends in vaccine talk of the 2019 COVID-19 Pandemic"

![NLP-image.png](https://github.com/iambindupriya/COVID-19-Vaccine-talk-analysis-using-NLP/blob/main/image/NLP-image.jpeg)

---

## Repo Content
- <b>[Data] (https://github.com/iambindupriya/COVID-19-Vaccine-talk-analysis-using-NLP/blob/main/Data)</b> - The dataset used in this project.
- <b>[images](https://github.com/iambindupriya/COVID-19-Vaccine-talk-analysis-using-NLP/tree/main/image)</b> - Various plots and images used in the documents found in this repo.
- <b>[Vaccine-SentimentAnalysis.ipynb](https://github.com/iambindupriya/COVID-19-Vaccine-talk-analysis-using-NLP/blob/main/Vaccine-SentimentAnalysis%20.ipynb)</b> - The main Jupyter Notebook containing the sentiment analysis for this project.
- <b>[README.md](README.md)</b> - A description of the project goals, process, and results.
- <b>[Presentation](https://github.com/iambindupriya/COVID-19-Vaccine-talk-analysis-using-NLP/blob/main/%E2%80%9CSentiment%20analysis%20of%20covid-19%20vaccine%20tweets%E2%80%9D.pptx)</b> -The PowerPoint of this project.

---

## Table of Content
- <b>[Overview](https://github.com/iambindupriya/COVID-19-Vaccine-talk-analysis-using-NLP/blob/main/README.md#overview)
- <b>[Goals](https://github.com/iambindupriya/COVID-19-Vaccine-talk-analysis-using-NLP/blob/main/README.md#goals)
- <b>[Motivation and Background](https://github.com/iambindupriya/COVID-19-Vaccine-talk-analysis-using-NLP/blob/main/README.md#motivation-and-background)
- <b>[Data](https://github.com/iambindupriya/COVID-19-Vaccine-talk-analysis-using-NLP/blob/main/README.md#data)
- <b>[Limitation](https://github.com/iambindupriya/COVID-19-Vaccine-talk-analysis-using-NLP/blob/main/README.md#limitation)
- <b>[Modeling](https://github.com/iambindupriya/COVID-19-Vaccine-talk-analysis-using-NLP/blob/main/README.md#modeling)
- <b>[Conclusion](https://github.com/iambindupriya/COVID-19-Vaccine-talk-analysis-using-NLP/blob/main/README.md#conclusion)
- <b>[Future Work](https://github.com/iambindupriya/COVID-19-Vaccine-talk-analysis-using-NLP/blob/main/README.md#future-work)
- <b>[Software Requirements](https://github.com/iambindupriya/COVID-19-Vaccine-talk-analysis-using-NLP/blob/main/README.md#software-requirements)
- <b>[Resource](https://github.com/iambindupriya/COVID-19-Vaccine-talk-analysis-using-NLP/blob/main/README.md#resource)
  

---
## Overview
  On global crisis like the COVID-19 epidemic, social media platforms like Twitter are a great way to share information and opinions. We use natural language processing and sentiment analysis tools to uncover information on public awareness of COVID-19 vaccine.We scrape tweets based on various keywords connected to vaccinations and health and safety issues following vaccination. This project will help policymakers better assess public reaction and plan vaccination campaigns, as well as health and safety measures, in the midst of the ongoing global health crisis.
  
  
## Goals
For our project, we want to draw conclusions about public sentiments towards the vaccination outlook when vaccinations become widely available to the population during the COVID-19 pandemic. 
We will perform a time series forecasting on the vaccination scenario of the USA and predict the percentage of the population that will be vaccinated by a certain timeline.

## Motivation and Background
  Sentiment analysis (also known as opinion mining or emotion AI) is the use of natural language processing, text analysis, computational linguistics, and biometrics to systematically identify, extract, quantify, and study affective states and subjective information. Sentiment analysis is widely applied to voice of the customer materials such as reviews and survey responses, online and social media, and healthcare materials for applications that range from marketing to customer service to clinical medicine.
  
  The Coronavirus disease-19 outbreak is a public health emergency of international concern. The COVID-19 pandemic is different from any previous pandemic. The variability of symptoms and the spread of the virus have led to an unprecedented speed of transmission. With the rapid increase in the number of confirmed cases, about 100,000 people are diagnosed every day. Vaccines may be the most effective way to suppress the spread of the virus. However, the public's attitude towards vaccines affects the vaccination rate and the time when the epidemic is over. Therefore, understanding the public's sentiments on vaccines is of vital importance to vaccination and epidemic control.
![word.png](https://github.com/iambindupriya/COVID-19-Vaccine-talk-analysis-using-NLP/blob/main/image/word.png)

## Research Questions
1. Is there a significant change in people's sentiment about vaccination?

2. Among the negative sentiment, what do people care most about? 

3. Performing a time series forecasting. 
  
## Data
Data will be gathered by scraping Twitter over various timeframes to get a wide variety of tweets related to the search term “COVID-19 Vaccine”, and various other related terms such as “COVID Vaccine” or “Moderna Vaccine”.  Data gathered will include information such as the time of the tweet, the language of the tweet, the text within it, and potentially even the geodata of the tweet. 
Data was originally planned to be collected using the Tweepy library in python.
  
The dataset will likely need to be cleaned for the following reasons:
Retweeting may cause some tweets to appear more than once
Non-standard characters such as Emojis being present
Spelling errors in tweets may throw off any NLP.
## Limitation
- Tweepy limits the amount of scraping at a time to 3200 individual tweets
- Tweepy cannot get tweets in a range via datetime, only by date
- Retweets in Tweepy are limited to only 140 characters before they are cut off
- In response to this, we have transferred to using the snscrape library to gather our data
  - The benefits of this are that snscrape has no such limitations on how it gathers the data, and has shown to be much more efficient at doing so. 
  - Columns of the dataframe include: url, date, content, user, lang, likeCount, retweetCount, and hashtags.


## Modeling

  
  
## Conclusion
  
  
## Future Work

  

## Software Requirements
<pre>
Languages    : Python 3.9.0
Tools/IDE    : Anaconda, Colab
Libraries    : numPy,pandas, matplotlib, seaborn, datetime, scikit-learn,warning 
</pre>

 <pre>
Duration     : October - December 2021
Last Update  : 10.13.2021
</pre>

## Resource
- <b>[An analysis of COVID-19 vaccine sentiments and opinions on Twitter](https://www.ijidonline.com/article/S1201-9712(21)00462-8/fulltext)
- <b>[COVID-19 Vaccination Awareness and Aftermath: Public Sentiment Analysis on Twitter Data and Vaccinated Population Prediction in the USA](https://www.mdpi.com/2076-3417/11/13/6128)
- <b>[Public Perception of the COVID-19 Pandemic on Twitter: Sentiment Analysis and Topic Modeling Study](https://publichealth.jmir.org/2020/4/e21978/)


