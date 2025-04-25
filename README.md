# News2Topics - LDA-based Topic Modeling

This project performs unsupervised topic modeling on a collection of news articles using Latent Dirichlet Allocation (LDA). It extracts underlying themes from headlines and content, helping to uncover hidden structures and trends in news data.

## 📌 Features

- Combines and cleans news text from multiple sources
- Tokenizes, removes stopwords, and preprocesses text
- Builds a dictionary and corpus using `gensim`
- Trains an LDA model to identify key topics
- Visualizes topics and outputs top keywords per topic
- Generates a final merged dataset for downstream use

---

## 📂 Dataset

The project uses dataset:
- `input.csv`: Contains columns like `URL`, `Date`, `Headline`, `Content`, `Portal`, etc.

---

## 🔍 Topic Modeling Process

- Preprocessing: Tokenization, lowercasing, removal of punctuation and stopwords
- Dictionary and Bag-of-Words construction
- Training with LDA (`gensim.models.LdaModel`)
- Topic visualization (optionally using `pyLDAvis`)

---

## 📊 Sample Topics Output

```python
topics = { 
    1: 'said, road, news, accidents, people, bus, police, vehicles, star, daily',
    2: 'road, said, news, police, daily, accident, star, around, accidents, also',
    3: 'police, injured, said, bus, upazila, news, killed, around, hospital, people',
    4: 'said, police, star, news, daily, accident, road, dhaka, bus, injured',
    5: 'said, police, news, road, daily, mymensingh, bridge, truck, star, bangladesh',
}
