# MovieLens-Recommender

A machine learning-based movie recommendation system that suggests films based on user ratings and movie titles. The system uses collaborative filtering and content-based approaches to provide personalized movie recommendations.
Features

Movie search by title
Get detailed movie information
User-based movie recommendations
Ratings distribution visualization

Technologies Used

Python 3.x
Pandas for data manipulation
Scikit-learn for TF-IDF vectorization
NumPy for numerical operations
Matplotlib for visualizations

Installation

Clone the repository:

bashCopygit clone https://github.com/ZannatKeya07/movielens-recommender.git
cd movielens-recommender

Install required packages:

bashCopypip install pandas numpy scikit-learn matplotlib

Download the MovieLens dataset and place movies.csv and ratings.csv in the project directory.

Usage
pythonCopy# Search for movies
results = search_movies("Toy Story")

# Get movie details
details = get_movie_details("Toy Story")

# Get recommendations based on movie ID
recommendations = find_user_recommendations(movie_id=1)
How It Works

Movie Search: Uses TF-IDF vectorization and cosine similarity to find movies matching the search query.
Recommendations: Implements collaborative filtering by:

Finding users who rated the target movie highly
Identifying other movies these users rated well
Calculating recommendation scores based on user ratings

Dataset
The system uses the MovieLens dataset containing:

Movie information (ID, title)
User ratings (user ID, movie ID, rating)

