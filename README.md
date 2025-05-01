# 🎬 Movie Recommender System using Machine Learning

A **Content-Based Movie Recommender System** built with Machine Learning techniques using the TMDB dataset.  
This project suggests movies similar to a user-selected title by analyzing movie metadata like genres, cast, crew, and keywords.

---

## 📖 About the Project

The goal of this project is to develop a machine learning-based recommendation engine that:

- Analyzes movie metadata (genres, cast, director, keywords, etc.)
- Computes similarity scores between movies
- Recommends the most similar movies to the selected title

> This is a **Content-Based Filtering** system — recommendations are made based on the **features of the selected movie**, not user preferences.

---

## 🛠 Project Pipeline

### 🔹 1. Data Collection
- Dataset: [TMDB Movie Metadata](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)
- Movie details include: `title`, `overview`, `genres`, `keywords`, `cast`, and `crew`

### 🔹 2. Data Preprocessing
- Cleaned and combined relevant features into a single text string
- Removed null/missing values
- Optional: Tokenization and Stemming

### 🔹 3. Feature Extraction
- Created a **Bag of Words** model using `CountVectorizer`
- Converted movie descriptions into numerical vectors

### 🔹 4. Recommendation System
- For a selected movie, returns **Top 5** most similar movies based on cosine similarity scores

### 🔹 5. Deployment (Optional)
- Built an interactive UI using **Streamlit**

---

## 🧠 Model Details

### Feature Engineering
- Combined columns: `genres`, `keywords`, `cast`, `crew`, and `overview`
- Processed into a single descriptive text per movie
