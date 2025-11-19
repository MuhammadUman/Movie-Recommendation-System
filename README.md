🎬 Movie Recommendation System (Machine Learning)

(You need to download "movie_list.pkl" and "similarity.pkl" for this to work)

This repository contains a content-based Movie Recommendation System built using Machine Learning and deployed with Streamlit. The system analyzes movie metadata, converts text features into numerical vectors, and uses Nearest Neighbors similarity to recommend movies similar to a selected title. The project includes full preprocessing, model building, and an interactive user interface.

🚀 Features

Content-Based Filtering
Recommends movies based on textual metadata such as overview, genres, cast, keywords, and crew.

Efficient Data Preprocessing
Handles missing values, merges relevant attributes, normalizes text fields, and constructs a unified feature called "tags".

Text Vectorization
Uses techniques like CountVectorizer or TF-IDF Vectorizer to transform text into numerical representations suitable for similarity calculation.

Nearest Neighbors Similarity
Computes distances between movie vectors using cosine similarity and KNN to identify the closest matches.

Interactive Streamlit Interface
Provides an easy-to-use interface where users:

Select a movie from a dropdown

Receive five recommended movies

View corresponding movie posters retrieved via the TMDB API

Model Serialization
Preprocessed movie data and similarity matrices are stored using pickle for fast loading and deployment.

How It Works:

Load and clean raw movie metadata.

Combine relevant text attributes into a single "tags" feature.

Vectorize tags using scikit-learn vectorization methods.

Compute pairwise similarities using Nearest Neighbors.

For any selected movie, retrieve the most similar movies.

Display recommendations and posters through Streamlit.
