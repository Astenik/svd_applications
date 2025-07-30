# svd_applications
This repository contains several practical applications of Singular Value Decomposition (SVD) in data science and machine learning, implemented in Python.
# Contents

# 1. MOVIE RECOMMENDER
# Description
This project builds a personalized movie recommendation system by combining the Movielens dataset with a curated list of Armenian films. The user provides ratings for movies they've seen, and the system recommends new titles using an SVD-based collaborative filtering model.

# Instalation
To run in Google Colab, install the following packages:

!pip install numpy==1.24.4 scipy==1.10.1
!pip install scikit-surprise --no-binary scikit-surprise

Download the Movielens dataset:

!wget https://files.grouplens.org/datasets/movielens/ml-latest-small.zip
!unzip ml-latest-small.zip

# Project structure

├── ml-latest-small/              Movielens dataset
│   ├── movies.csv
│   └── ratings.csv
├── recommender.py               Core logic with all functions
├── main.ipynb                    Notebook or Colab script
└── README.md

# How It Works
1. The user enters movies they've seen and their ratings, for example:

  The Color of Pomegranates, 4.5  
  We and Our Mountains, 5.0  
  The Promise, 4.0  
  
2. If a movie is not in the dataset, the system asks for its genre and adds it.
3. The model is trained (or retrained) including these ratings.
4. Personalized recommendations are generated using SVD.

# Algorithm & Features
1. SVD (Singular Value Decomposition) from scikit-surprise
2.Real Movielens data + synthetic ratings for Armenian films
3. Interactive user input for new ratings
4. Dynamic expansion of the movie database

# Sample Output
Recommended Movies:
1. Old Armenian Film 1 (4.82)
2. The Matrix (4.76)
3. Piece of Sky (4.68)


# Author
Astenik Hovhannisyan (https://github.com/Astenik)
