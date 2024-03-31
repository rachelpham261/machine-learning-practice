# Movie Recommendation using K-Nearest Neighbors (KNN)

This repo implements a simple Movie Recommender System using the K-Nearest Neighbors (KNN) algorithm. This system recommends new movies to users based on similarities between movies in a database and the movie the user just watched (or is watching). This README provides details about the setup, usage, and customization of the recommendation model.

## Setup
The code requires `pandas` for loading and processing data, `sklearn` for the implementation of the KNN algorithm, and `matplotlib` for visualization. We specifically use the following versions of the packages:
- Python: 3.11.5
- Pandas: 1.26.3
- Sklearn: 1.2.2
- Matplotlib: 3.8.0


Once you have the prerequisites installed, download the file `knn.ipynb`, a notebook that implements all steps with careful explanation for data loading, EDA, fitting the KNN model, and applying the model to a new movie.

## Dataset details
The data in `movies_recommendation_data.csv` is a dataframe of 30 movies with the following columns:
- Movie ID: Unique identifier for each movie.
- Movie Name: Title of the movie.
- IMDB Rating: Rating by critics from IMDB.
- Biography: 1 means this is Biography, 0 means this is not Biography.
- Drama: 1 means this is Drama, 0 means this is not Drama.
- Thriller: 1 means this is Thriller, 0 means this is not Thriller.
- Comedy: 1 means this is Comedy, 0 means this is not Comedy.
- Crime: 1 means this is Crime, 0 means this is not Crime.
- Mystery: 1 means this is Mystery, 0 means this is not Mystery.
- History: 1 means this is History, 0 means this is not History.
- Label: The label of each movie. However, in this movie recommender system, the label values are all zeros because the label information is not needed for extracting the nearest movies.

## EDA
We first visualize the distribution of each column to gain a better understanding of the data. We visualize the histogram of IMDB Rating, as this is a continuous variable, and the bar plot of other columns as they are discrete (0 and 1 values).

## KNN
The K-Nearest Neighbors (KNN) algorithm provides recommendations based on similarities of a new movie and the existing movies in the dataset. In this project, we implement KNN with `n_neighbors=5`, which means we consider the five closest neighbors when making recommendations for a particular movie.

We consider "The Post" the movie that the user likes, and use KNN to find the nearest movies to "The Post" to recommend to this user.