# Music Recommendation System

## Overview

This project implements a *Music Recommendation System* combining *Content-Based Filtering, **Collaborative Filtering, and **KNN-Based Recommendations*. It leverages machine learning techniques to recommend songs based on lyrics, user preferences, and user-item interactions.



## Project Description

The Music Recommendation System leverages a combination of advanced machine learning techniques to provide users with personalized song recommendations. This system integrates Content-Based Filtering, Collaborative Filtering, and KNN-Based Recommendations, offering a holistic approach to suggesting songs based on song attributes, user interactions, and similarity to other users.
The project uses lyrics-based content filtering and user interaction data to deliver customized recommendations, ensuring that the system adapts to both individual preferences and popular trends.


## Features

### Content-Based Recommender
- *Objective*: To recommend songs based on their similarity in lyrics.
- *Approach: Utilizes **TF-IDF vectorization* to transform song lyrics into numerical vectors and computes similarity using *cosine similarity*.
  - Songs with similar lyrical content are recommended.
  - Can be personalized to the user by analyzing the lyrics of their most listened-to songs.

### Collaborative Filtering Recommender
- *Objective*: To suggest songs based on the listening patterns of similar users.
- *Approach: Implements the **Singular Value Decomposition (SVD)* algorithm from the *Surprise* library. This technique decomposes the user-item interaction matrix into singular values and helps uncover hidden relationships between users and songs.
  - The system identifies patterns in user behavior and recommends songs based on these patterns.
  - Works well for suggesting songs based on the collective preferences of similar users.

### KNN-Based Recommender
- *Objective*: To recommend songs based on user similarity.
- *Approach: Uses **K-Nearest Neighbors (KNN)* to find similar users based on their song preferences.
  - The system creates a *user-item interaction matrix*, which captures user behavior such as song likes or listens.
  - It then identifies users with similar interaction patterns to make personalized song recommendations.

### Visualization Functions
The system includes a variety of visualizations to help analyze and interpret the data:
- *Pie charts* for song genre distribution.
- *Bar charts* to visualize the most popular songs.
- *Histograms* showing the distribution of user interactions (e.g., how many times a song was played).
- *Heatmaps* to show correlations between users and songs.

## Datasets

### 1. Content-Based Dataset:
- *songdata.csv*: This dataset contains the following attributes:
  - *Song ID*
  - *Song Title*
  - *Artist*
  - *Lyrics* (Text data used for content-based recommendations)
  
### 2. Collaborative Filtering Dataset:
- *Bollywood-Songs-Dataset(2017-23).csv*: This dataset contains synthetic user interaction data, such as:
  - *User ID*
  - *Song ID*
  - *Listen Count* (How many times a user listened to a particular song)
  - This data is used for building collaborative filtering models.
 

# Prerequisites
The system requires the following Python libraries:

# Installing Python 3.x (Recommended version: 3.7 or higher)

### pandas - Data manipulation and analysis
### numpy - Numerical computations
### matplotlib - Plotting and visualization
### seaborn - Statistical data visualization
### scikit-learn - Machine learning algorithms
### scipy - Scientific computing
### surprise - A library for building and analyzing recommender systems
# Install the required libraries
```bash 
pip install numpy 
pip install matplotlib
pip install seaborn
pip install scikit-learn
pip install scipy 
pip install surprise
