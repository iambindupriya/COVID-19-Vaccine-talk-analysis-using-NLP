# COVID-19-Vaccine-talk-analysis-using-NLP
"Understanding people's sentiment, trends in vaccine talk of the 2019 COVID-19 Pandemic"

## Table of Content
- <b>[Overview](https://github.com/iambindupriya/COVID-19-Vaccine-talk-analysis-using-NLP/blob/main/README.md#overview)
- <b>[Goals](https://github.com/iambindupriya/COVID-19-Vaccine-talk-analysis-using-NLP/blob/main/README.md#goals)
- <b>[Data](https://github.com/iambindupriya/COVID-19-Vaccine-talk-analysis-using-NLP/blob/main/README.md#data)
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
Spelling errors in tweets may throw off any NLP


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
Duration     : October 2021
Last Update  : 10.5.2021
</pre>

## Resource
- <b>[An analysis of COVID-19 vaccine sentiments and opinions on Twitter](https://www.ijidonline.com/article/S1201-9712(21)00462-8/fulltext)
- <b>[COVID-19 Vaccination Awareness and Aftermath: Public Sentiment Analysis on Twitter Data and Vaccinated Population Prediction in the USA](https://www.mdpi.com/2076-3417/11/13/6128)
- <b>[Public Perception of the COVID-19 Pandemic on Twitter: Sentiment Analysis and Topic Modeling Study
Public Perception of the COVID-19 Pandemic on Twitter: Sentiment Analysis and Topic Modeling Study
Authors of this article:](https://publichealth.jmir.org/2020/4/e21978/)


