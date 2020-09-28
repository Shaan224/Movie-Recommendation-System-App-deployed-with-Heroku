# Movie-Recommendation-System-App-deployed-with-Heroku


## Introduction

In this repo I have built a Content Based Movie Recommendation System and deployed it on Heroku.

## Datasets 
* [**IMDB 5000 Movie Dataset**](https://www.kaggle.com/carolzhangdc/imdb-5000-movie-dataset)
* [**The Movies Dataset**](https://www.kaggle.com/rounakbanik/the-movies-dataset)
* [**Scraping list of 2018 movies**](https://en.wikipedia.org/wiki/List_of_American_films_of_2018)
* [**Scraping list of 2019 movies**](https://en.wikipedia.org/wiki/List_of_American_films_of_2019)
* [**Scraping list of 2020 movies**](https://en.wikipedia.org/wiki/List_of_American_films_of_2020)

The details of the movies(title, genre, runtime, rating, poster, etc) are fetched using an API by TMDB, [**API**](https://www.themoviedb.org/documentation/api), and using the IMDB id of the movie in the API, I did web scraping to get the reviews given by the user in the IMDB site using beautifulsoup4 and performed sentiment analysis on those reviews.

Movie recommendations are made on the basis of similar Actors, Director(s), Language, Genres and Plot Keywords.

Similarity score is value between 0 to 1 which determines how similar two objects are on a scale of 0 to 1. Higher the score -> Higher the similarity between the objects.
There are many ways to calculate the similarity scores for example - Euclidean Distance, Manhattan Distance, Cosine Similarity etc.

In this model we are using Cosine Similarity to recommmend the Top 10 movies based on their similarity scores.

After building the model I deployed this model on **Heroku** using **Flask**

Deployed Model - [**Heroku**](https://movie-recommendationapp.herokuapp.com/)

## Tools And Technologies

* NLTK libraries - Is used for text wrangling and preprocessing of the reviews. Tokenization, Lemmatization and Stopword removal.
* Matplotlib and Plotly - For visualization and creating interactive plots.
* Sklearn Countvectorizer - To create Term-Document Matrix
* Pandas and Numpy - For Data Manipulation and Text Cleaning
* Flask -  For deploying the machine learning model

To read more about recommendation systems [**click here**](https://builtin.com/data-science/recommender-systems)


## Scope of Improvements

Still working on making better recommendation and creating the interface for smooth and interactive.
