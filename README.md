# COVID-19-Vaccine-talk-analysis-using-NLP
"Understanding people's sentiment, trends in vaccine talk of the 2019 COVID-19 Pandemic"

![NLP-image.png](https://github.com/iambindupriya/COVID-19-Vaccine-talk-analysis-using-NLP/blob/main/image/NLP-image.jpeg)

---

## Repo Content
- <b>[Data](https://github.com/iambindupriya/COVID-19-Vaccine-talk-analysis-using-NLP/blob/main/Data)</b> - The dataset used in this project.
- <b>[images](https://github.com/iambindupriya/COVID-19-Vaccine-talk-analysis-using-NLP/tree/main/image)</b> - Various plots and images used in the documents found in this repo.
- <b>[Vaccine Talk.ipynb](https://github.com/iambindupriya/COVID-19-Vaccine-talk-analysis-using-NLP/blob/main/VaccineTalk.ipynb)</b> - The main Jupyter Notebook containing the sentiment analysis for this project.
- <b>[README.md](README.md)</b> - A description of the project goals, process, and results.
- <b>[Presentation](https://github.com/iambindupriya/COVID-19-Vaccine-talk-analysis-using-NLP/blob/main/Slides.pptx)</b> -The PowerPoint of this project.

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
 This is a quantitative analysis of COVID-19 vaccination in the aftermath of the 2020 COVID-19 outbreak. Using a Twitter dataset, we examine public opinion on COVID-19 vaccinations. Despite some side effects observed in various vaccines, we find that the public sentiment is more positive than negative.
From the perspective of negative emotions, people are skeptical about the safety of vaccines, and they are more worried about whether they will have side effects after vaccination, and lead to other diseases or deaths. In addition to widely spread rumors, improving the safety of vaccines and how to effectively promote the safety of vaccines is also a difficult problem for health officials to face. 
  
In addition, in the negative sentiments, we found a special group called anti-vaxxers.. People who feel vaccines are unsafe and infringe on their human rights are known as anti-vaxxers. They usually dispute the existence or validity of the science that supports its widespread use.  Although the anti-vaccine organization is small, their online communication strategy is very effective and far-reaching, which is worrying. With the outbreak of the COVID-19 crisis, these people have realized that this virus can take anyone's life. People of any age, although high-risk groups are particularly vulnerable, there are also many healthy people who get sick and die from the virus. Some anti-vaxxers have begun to try vaccination.
  
Excluding those anti-vaxxers who deliberately spread rumors, health officials need to understand the concerns of those who oppose vaccines. To curb the spread of anti-vaccine sentiment, health officials need to understand how it formed. They need to work hard to reduce the dissemination of incorrect information on social media and provide correct guidance to the public in a timely manner. With concrete evidence to prove the credibility of the vaccine, we believe that more and more anti-vaccine people will start to vaccinate

  
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


