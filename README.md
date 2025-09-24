Spotify Popularity Prediction
Description

This project aims to predict whether a song is popular or not based on its attributes from Spotify data. Popularity is defined as appearing in at least 5,000 playlists. The goal is to investigate how handling class imbalance affects model performance.

Research Question

Can we use machine learning to predict a song’s popularity, and how does dataset balancing impact model performance?

Dataset

The dataset consists of song data collected from Spotify, including features such as danceability, energy level, tempo, and other musical attributes. The target variable is binary: "Popular" (≥5,000 playlists) or "Not Popular" (<5,000 playlists).

You can download the dataset used in this project from Kaggle:
https://www.kaggle.com/datasets/ahmadrazakashif/spotify-popularity-songs 

Methodology

Data Processing – Cleaning and preparing the dataset.

Model – Logistic Regression.

Handling Class Imbalance – RandomOverSampler.

Evaluation – Accuracy, Recall, F1-score, and ROC curves.

Results

After balancing with RandomOverSampler, the macro‑F1 score increased from approximately 0.67 to around 0.77, and recall for the popular class rose from about 0.31 to approximately 0.66. This demonstrates that the model becomes better at identifying popular songs. ROC curves before and after balancing show a clear improvement across different threshold values.

Conclusion

We demonstrated that dataset balancing significantly impacts the model’s ability to predict the minority class (popular songs). Logistic Regression combined with RandomOverSampler considerably improved model performance. The results confirm that class imbalance is an important factor to address in machine learning problems where the minority class is business-critical.

Limitations

- Dataset size.

- Definition of “popular.”

- External factors such as marketing.

- Suggestions for Improvement

- Use advanced balancing techniques such as SMOTE.

- Test other models (Random Forest, XGBoost).

- Hyperparameter optimization.

- Stratified cross-validation.
