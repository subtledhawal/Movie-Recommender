# Movie Recommendation System

This project is a Movie Recommendation System built using Python and hosted locally via PyCharm. The system employs data visualization and data modelling techniques to provide movie recommendations based on user input. The dataset contains information about various movies, including genres, actors, directors, and more. The system uses a similarity-based model to recommend movies similar to the ones the user has selected.


![image](https://github.com/user-attachments/assets/c254d894-c214-478f-b2af-94810cf4a4af)



## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Modeling](#modeling)
- [Visualization](#visualization)

## Features
- **Movie Recommendations**: Get movie recommendations based on a selected movie title.
- **Data Visualization**: Visualize the relationships between movies, genres, and other features.
- **Similarity Calculation**: Uses cosine similarity to find similar movies based on selected features.
- **Hosting**: The system is hosted on a local server via PyCharm for easy deployment.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/subtledhawal/Movie-Recommender.git
    cd Movie-Recommender
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the server:
    ```bash
    python app.py
    ```

4. Access the web app locally:
    ```
    http://127.0.0.1:5000
    ```

## Usage
1. **Data Loading**: The system loads a preprocessed dataset of movies.
2. **Recommendation**: Input a movie title to get a list of similar movies.
3. **Data Visualization**: Explore various data visualizations to gain insights into movie genres, actors, and directors.

### Example
You can get recommendations by selecting a movie title like "Gandhi" and the system will suggest similar movies such as:
- *Gandhi, My Father*
- *The Wind That Shakes the Barley*
- *A Passage to India*

## Dataset
Dataset used: https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata
The dataset includes:
- Movie titles
- Genres
- Tags (e.g., action, comedy)
- Actors and directors

The dataset has been cleaned and preprocessed, and it is stored in `movie_list.pkl` and `movie_dict.pkl` files.

## Modeling
The system uses cosine similarity on the movie feature vectors to calculate similarity between movies. The features include genres, actors, and tags.

### Libraries Used
- **pandas**: For data manipulation and analysis
- **scikit-learn**: For computing cosine similarity
- **pickle**: For saving and loading models
- **Flask**: For hosting the recommendation engine as a web app

## Visualization
The project includes visual representations of relationships between different movie attributes:
- **Genres**: Distribution of movie genres.
- **Actor Appearances**: Frequency of actors in various genres.

