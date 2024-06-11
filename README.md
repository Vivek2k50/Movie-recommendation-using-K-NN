Movie Recommendation System using K-NN
Description:
This project implements a movie recommendation system using the K-Nearest Neighbors (K-NN) algorithm. The system recommends movies based on a combination of features including genres, keywords, tagline, cast, and director.

Libraries and Tools Used:
Python
NumPy
Pandas
Scikit-learn
Difflib

Data Preprocessing:
Loading Data: The dataset containing movie information is loaded using Pandas.
Feature Selection: The relevant features for recommendation are selected: 'genres', 'keywords', 'tagline', 'cast', and 'director'.
Handling Missing Values: Null values in the selected features are replaced with empty strings.
Combining Features: The selected features are combined into a single text string for each movie

Model Building:
Feature Vectorization: The combined text features are converted into feature vectors using TF-IDF vectorization.
K-NN Model Training: A K-Nearest Neighbors model is trained using the cosine similarity metric to find the most similar movies.

Movie Recommendation Function:
The function get_knn_recommendations(movie_name) is implemented to:

Find Closest Match: Identify the closest match for the given movie name from the dataset.
Retrieve Movie Index: Find the index of the movie in the dataset.
Calculate Similarity: Compute the similarity between the given movie and all other movies using the K-NN model.
Recommend Movies: Print the titles of the 30 most similar movies.

Usage:
To get movie recommendations, run the notebook and enter your favorite movie name when prompted. The system will output a list of movies similar to your favorite movie.

# Get recommendations for a specific movie
movie_name = input('Enter your favourite movie name: ')
get_knn_recommendations(movie_name)

Conclusion:
This project successfully builds a movie recommendation system using K-NN, providing relevant movie suggestions based on various features. The approach can be further enhanced by incorporating additional features or using more advanced recommendation algorithms.
