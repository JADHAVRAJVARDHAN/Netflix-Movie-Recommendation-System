# **Netflix-Movie-Recommendation-System**
The project in the notebook is a movie recommendation system. It aims to predict movies that a user might enjoy based on their past ratings and the ratings of other users.

**Here's a breakdown:**

**Project Goal:**

Build a system that recommends movies to users based on their preferences and the preferences of similar users.
The notebook uses data from Netflix consisting of user ratings on movies.
Algorithm Used:

The primary algorithm used for building the recommendation system is SVD (Singular Value Decomposition).

SVD is a matrix factorization technique that is widely used in collaborative filtering for recommendation systems.
It decomposes the user-item rating matrix into three matrices, revealing latent factors that represent underlying preferences and patterns.
These latent factors are then used to predict the rating a user would give to an item they haven't seen before.
Key Steps in the Notebook:

**Data Loading and Preprocessing:**

Reads movie ratings data.
Performs data cleaning and filtering to remove inactive users and unpopular movies.
Model Building:

Uses the surprise library to implement SVD.
Trains the model on a portion of the data.
**Recommendation Generation:**

Filters the data to find movies a specific user liked.
Predicts the ratings for all other movies for that user using the SVD model.
Sorts the predictions to recommend the top movies with the highest predicted ratings.
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
In summary, this project implements a movie recommendation system using the SVD algorithm. It involves data preprocessing, model building, and recommendation generation steps.

I hope this helps! Let me know if you have any more questions.
