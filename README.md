## Movie Recommender System

# Overview
This project implements a Movie Recommender System using collaborative filtering. It recommends movies similar to the one selected by the user, based on a dataset of movies and their similarity scores.

# How It Works
The system uses a dataset stored in a pickle file (movie_list.pkl) containing movie titles and IDs, and another pickle file (similarity.pkl) containing a similarity matrix between the movies. Here's a breakdown of the functionality:

Movie Selection: Users can select a movie from a dropdown menu.
Recommendation: Upon selecting a movie and clicking the "Show Recommendation" button, the system fetches and displays five recommended movies. It does this by computing similarity scores between the selected movie and all others, then selecting the top 5 most similar movies.
Display: For each recommended movie, the system displays the movie title and its poster retrieved from "The Movie Database" API using the fetch_poster function.

# Code Files

1.Main Application (app.py):

Imports necessary libraries and defines functions for fetching movie posters (fetch_poster) and generating recommendations (recommend).
Loads precomputed data (movies and similarity) from pickle files.
Uses Streamlit to create a user interface where users can interact with the recommender system.

2.Supporting Scripts:

Data Preparation (data_preparation.py): This script preprocesses movie data and computes similarity scores between movies, storing results in pickle files used by app.py.

# Requirements
Python 3.x
Streamlit
Requests
Pickle

# Setup Instructions

1.Clone the repository:

bash code:
git clone https://github.com/yourusername/handwritten-digit-recognition.git
cd movie-recommender-system

2.Install the required libraries:

bash code:
pip install -r requirements.txt

3.Run the application:

bash code:
streamlit run app.py

# Future Improvements
Implement user-based or item-based collaborative filtering for personalized recommendations.
Enhance UI/UX with more interactive features.
Deploy the application using cloud services for broader accessibility.

# Credits
Dataset: The movie dataset and similarity scores were obtained and preprocessed using techniques from collaborative filtering.
API: Movie posters are fetched from "The Movie Database" API.
Feel free to contribute to enhance the system or suggest improvements! Happy movie recommending! 🎬
