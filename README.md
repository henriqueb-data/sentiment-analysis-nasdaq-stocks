# 📘 NASDAQ Stocks – Sentiment Analysis  
Analyze financial news sentiment related to NASDAQ-listed stocks to explore how textual data can support investment decision-making.

---

## 🔍 Overview  
- **Goal:** Build and evaluate a sentiment analysis model to classify financial news related to NASDAQ stocks.  
- **Problem Type:** Natural Language Processing (Sentiment Classification)  
- **Dataset:** Financial news headlines and articles labeled by sentiment (negative, neutral, positive).

---

## 🧭 Context  
Investment firms process large volumes of financial news daily to understand market sentiment and anticipate stock price movements.  
Manual labeling and analysis of this information is time-consuming and costly.

This project applies sentiment analysis techniques to financial news data to evaluate model performance and explore how automated text analysis could support faster and more scalable investment workflows.

---

## 📊 Data Summary  
- **Target Variable:** News sentiment (negative, neutral, positive)  
- **Key Features:**  
  - Financial news text  
  - Derived text representations used for modeling  
- **Data Notes:**  
  - Multi-class sentiment classification  
  - Class imbalance between neutral, positive, and negative news  
  - Model performance differs significantly between training and unseen test data

---

## 🛠 Methods & Concepts Used  
- **Preprocessing:**  
  - Text cleaning and normalization  
  - Tokenization  
  - Text vectorization 

- **Modeling:**  
  - Supervised sentiment classification using different embedding strategies: **Word2Vec**, **GloVe**, and **Sentence Transformers**
  - Training vs. test performance comparison  

- **Techniques:**  
  - Model evaluation by class (negative, neutral, positive)  
  - Error analysis on unseen data  
  - Performance assessment under class imbalance  

---

## 💡 Actionable Insights  

- Although the sentiment analysis model performed well on the training data, it showed significantly weaker performance on unseen test data, particularly for **negative and positive news**, indicating limited generalization.

- Improving the **data collection strategy** by including more negative and positive news could help balance the dataset and potentially improve model performance.

- The sentiment analysis model could be **commercialized and sold to investment firms**, allowing them to automate sentiment labeling of financial news, reduce manual analysis costs, and react more quickly to market changes.

- As an alternative, investment firms could adopt **Large Language Models (LLMs)** to perform both sentiment analysis and news summarization, automating not only labeling but also identifying news likely to impact stock prices. While LLMs require more computational resources, running scheduled jobs (e.g., once per day) would be feasible for firms with access to GPUs.

- Despite the benefits of automation, firms should **frequently review model outputs**, as LLM-based and sentiment models may introduce issues such as hallucinations, inaccuracies, bias, or misinterpretation of nuanced language.

---

## 👤 Author  
**Henrique Barbosa**  
GitHub: https://github.com/henriqueb-data/
