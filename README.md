# YouTube Stance Analysis: Russia-Ukraine Conflict

This project focuses on analyzing YouTube comments to understand audience sentiments and stances on the Russia-Ukraine conflict. It leverages machine learning models for sentiment classification and clustering to provide insights into public opinion.

## Features

- **Data Collection**:  
  - Collected comments from YouTube videos using the YouTube Data API.
  - Extracted and structured data for analysis.

- **Data Preprocessing**:  
  - Cleaned and tokenized text data.
  - Removed non-English comments, special characters, and irrelevant data.
  - Applied TF-IDF for feature extraction.

- **Sentiment Analysis**:  
  - Classified comments as positive, negative, or neutral using Logistic Regression, SVM, and Naïve Bayes.
  - Used a majority vote ensemble for improved accuracy.

- **Clustering**:  
  - Applied K-means clustering on TF-IDF features.
  - Visualized clusters using PCA for insights into comment patterns.

## Workflow

1. **Data Collection**:  
   - Extracted YouTube comments using the YouTube Data API v3 and `googleapiclient`.
   - Fetched comments based on specific video IDs.

2. **Data Preprocessing**:  
   - Lowercased text and removed special characters, emojis, and URLs.
   - Tokenized text into bigrams and trigrams.
   - Applied stop-word removal and lemmatization.

3. **Modeling**:  
   - Trained Logistic Regression, SVM, and Naïve Bayes models.
   - Combined predictions using majority voting.
   - Accuracy: Logistic Regression (71%), SVM (71%), Naïve Bayes (65%).

4. **Clustering**:  
   - Applied K-means clustering to categorize comments into three groups.
   - Used PCA for 2D visualization of clusters.

5. **Insights**:  
   - Identified key topics, sentiments, and stances in the comments.
   - Provided actionable insights into public opinion and audience engagement.

## Results

- Sentiment analysis models achieved moderate accuracy with SVM performing the best.
- Clustering revealed patterns in audience reactions and opinions.

## Tools & Technologies

- Python
- Jupyter Notebook
- Libraries: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, Google API Client

## Future Work

- Train domain-specific sentiment analysis models for YouTube comments.
- Incorporate real-time sentiment monitoring.
- Explore multimodal analysis combining text and visual elements.

## License

This project is licensed under the [MIT License](LICENSE).

