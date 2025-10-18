# Mining Consumer Voices: A Sentiment Analysis of Financial Complaints Using NLP

This project analyzes consumer complaint data from the Consumer Financial Protection Bureau (CFPB) using Natural Language Processing (NLP). The goal is to extract insights from complaint narratives, classify sentiment, and identify trends in consumer satisfaction across financial products and companies.

---

##  Project Objectives

- Analyze and preprocess real-world consumer complaint data.
- Perform sentiment analysis on complaint narratives based on company responses.
- Extract key themes and concerns for different financial products using TF-IDF.
- Generate word clouds and summaries for each product category.
- Identify the best and worst-performing companies based on sentiment trends.

---

##  Dataset

**Source:** [CFPB Consumer Complaints](https://www.kaggle.com/datasets/sbhatti/consumer-finance-complaints)

**Key Features Used:**

- `consumer_complaint_narrative`
- `product`
- `company`
- `company_response_to_consumer`
- `submitted_via`
- `timely_response`
- `consumer_disputed?`

---

##  Methods & Tools

| Task                        | Libraries/Techniques                            |
|----------------------------|--------------------------------------------------|
| Data cleaning              | Pandas, NumPy                                    |
| Text preprocessing         | NLTK, Regex (`re`), string                       |
| Sentiment classification   | Rule-based mapping from company responses        |
| Keyword extraction         | TF-IDF (scikit-learn)                            |
| Visualization              | Matplotlib, WordCloud                            |
| Text summarization         | Sumy / Transformers (optional)                   |
| Development environment    | Google Colab                                     |

---

##  Preprocessing Steps

1. Drop rows with missing narratives for NLP.
2. Normalize text:
   - Lowercasing
   - Remove URLs, digits, punctuation
   - Tokenization
   - Stopword removal
   - Lemmatization
3. Clean and prepare separate datasets for:
   - **NLP-based Sentiment Analysis**
   - **Exploratory Data Analysis (EDA)**

---

##  Sentiment Analysis 
#### Use case1: 
For Credit card, consumers show the most positive sentiment toward First Data Corporation.

Key insights:
• Sentiment score: 0.072 (range: -1 to +1)
• Based on 5 complaints analyzed
• Customers frequently express satisfaction and good experiences with their credit card services

Rankings:
1. First Data Corporation
   Sentiment Score: 0.072
   Complaints Analyzed: 5

2. Boeing Employees' Credit Union
   Sentiment Score: 0.070
   Complaints Analyzed: 5

3. SunTrust Banks, Inc.
   Sentiment Score: 0.067
   Complaints Analyzed: 9

#### Use case2:
For Debt collection, consumers show the most negative sentiment toward The Phoenix Recovery Group.

Key insights:
• Sentiment score: -0.181 (range: -1 to +1)
• Based on 6 complaints analyzed
• Customers frequently express frustration and poor experiences with their debt collection services

Rankings:
1. The Phoenix Recovery Group
   Sentiment Score: -0.181
   Complaints Analyzed: 6

2. Servatus Corporation
   Sentiment Score: -0.185
   Complaints Analyzed: 6

3. Collections Acquisition Company, Inc.
   Sentiment Score: -0.357
   Complaints Analyzed: 9
________________________________________________________________________________

