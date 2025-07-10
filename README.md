# Twitter Entity Sentiment Analysis

##  Project Objective

This project analyzes sentiment patterns in Twitter data related to various entities (e.g., brands, games, platforms) to uncover public opinion and emotional tone. The aim is to preprocess, visualize, and classify sentiment using machine learning, enabling organizations to gain actionable insights into brand perception and audience attitudes.


##  Dataset

* **Source**: [Twitter Entity Sentiment Analysis on Kaggle](https://www.kaggle.com/datasets/jp797498e/twitter-entity-sentiment-analysis)
* **Files used**:

  * `twitter_training.csv`
  * `twitter_validation.csv`

Each record contains:

* `ID`, `Entity`, `Sentiment`, `Text`


##  Technologies & Libraries

* **Language**: Python
* **Libraries**:

  * `pandas`, `numpy` – data handling
  * `matplotlib`, `seaborn`, `wordcloud` – visualizations
  * `nltk` – text preprocessing
  * `sklearn` – vectorization, model training, evaluation


##  Workflow Summary

1. **Data Loading** – Combined training and validation datasets
2. **Cleaning & Preprocessing**:

   * Removed URLs, mentions, hashtags
   * Lowercased text and removed punctuation
   * Removed stopwords and applied lemmatization
3. **Exploratory Data Analysis**:

   * Sentiment and entity distributions
   * Word clouds per sentiment class
   * Entity-wise sentiment scores
4. **Feature Engineering** – TF-IDF vectorization
5. **Modeling** – Logistic Regression classifier with stratified train-test split
6. **Evaluation** – Classification report and confusion matrix


##  Key Visualizations

* Bar plots of sentiment and entity distributions
* Word clouds per sentiment category
* Sentiment score ranking across top entities

> **Note**: Some tweets in the dataset may contain foul or offensive language. These are kept intact for academic and analytical purposes only.


##  Model Performance

* **Classifier**: Logistic Regression
* **Accuracy**: \~91%
* **Evaluation**: Balanced classification report and confusion matrix analysis


##  Use Cases

* **Brand monitoring**: Understand how users perceive a product or service in real time.
* **Trend analysis**: Track changing sentiment over time for marketing strategy.
* **Customer support prioritization**: Identify spikes in negative sentiment toward specific entities.


##  Disclaimer

This dataset includes tweets from the public domain, some of which may include offensive or inappropriate content. The data has not been manually censored and is used here for educational and research purposes only.