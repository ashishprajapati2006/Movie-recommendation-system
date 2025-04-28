🎬 Movie Recommender System using Machine Learning
A content-based movie recommender system built with Machine Learning techniques using the TMDB dataset.

This project predicts and suggests movies similar to the user's selected movie based on key features such as genres, cast, crew, and keywords.


📖 About the Project
The goal is to create a recommendation engine that:

Analyzes movie metadata (genres, cast, director, etc.).

Computes movie-to-movie similarity scores.

Recommends top movies based on similarity.

This is a Content-Based Filtering recommender system — meaning it recommends movies based on the features of the movie selected.


🛠 Project Pipeline
Data Collection

Used TMDB dataset containing movie details (title, overview, genres, keywords, cast, crew).

Data Preprocessing

Cleaning and combining important features into a single text.

Handling missing values.

Tokenization and Stemming (optional).

Feature Extraction

Created a bag of words using CountVectorizer.

Transformed text data into numerical feature vectors.

Similarity Computation

Used Cosine Similarity to calculate similarity between movies.

Recommendation System

For a given movie, retrieve top 5 similar movies.

Deployment (Optional)

Built a simple web interface using Streamlit.


🧠 Model Details
Feature Engineering:

Combined important columns: genres, keywords, cast, crew, overview.

Processed into a single combined feature text.

Vectorization:

Used CountVectorizer (max_features=5000, stop_words='english').

Similarity Measure:

Applied Cosine Similarity between movie feature vectors.

Recommendation:

Retrieved top 5 movies based on highest cosine similarity scores.


📈 Results
Fast and accurate recommendations based purely on movie content.

Display of movie posters for better visual appeal.

Lightweight system suitable for further scaling.

Here are some sample pictures:
![image](https://github.com/user-attachments/assets/e6fc3c00-d3d7-4a51-bab9-9c7c5a2707e1)
![image](https://github.com/user-attachments/assets/9e297990-487b-4928-a6e2-491d463bba73)


The dataset link: https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata
