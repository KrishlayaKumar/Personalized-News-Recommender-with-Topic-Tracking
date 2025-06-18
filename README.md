# Personalized-News-Recommender-with-Topic-Tracking
Recommend relevant news articles based on the user's interests.

## 1. Understand the Problem:-

  1) Goal: Recommend relevant news articles based on the user's interests.
  2) Personalization: Based on reading history, clicked articles, and inferred preferences.
  3) Topic Tracking: Adjust user profile as interests evolve (e.g., more sports, less politics over time).

##  2. Collect the Data:-

  1) MIND Dataset – Microsoft News Dataset (very popular for news recommendation)
  2) News Category Dataset – Kaggle dataset with news headlines and categories: Kaggle link

## 3. Preprocess News Articles:-

  1) Clean text (remove stopwords, punctuation).
  2) Use NLP for:
     1) Tokenization
     2) Named Entity Recognition (NER)
     3) Topic Modeling (LDA or NMF)
     4) Text Embeddings (BERT, TF-IDF, etc.)
        
##  4. Build User Profiles:-

  1) Store articles they clicked or liked
  2) Extract topics/keywords from those articles
  3) Create a user embedding = average of their article embeddings

## 5. Recommendation Engine :-
  Content-based Filtering:
    1) Compute cosine similarity between user profile and article embeddings.
    2) Recommend top-N closest articles.

## 6. Topic Tracking:-
  1) Maintain a history of topic scores per user (e.g., 30% tech, 20% sports).
  2) Update scores dynamically as the user interacts.
  3) Use a decay factor so old preferences fade over time.

## 7. Build Frontend :-
Use Streamlit or Flask to show:
  1)Top recommended articles.
  2)User interest trends (e.g., pie chart of topics)
  3)Search functionality




