# Netflix Movie Recommendation System

The Netflix Movie Recommendation System is a project aimed at predicting movies that users might enjoy based on their past ratings and the preferences of other users. It leverages collaborative filtering techniques to provide personalized movie recommendations.

---

## **Project Goal**
The primary objective is to build a recommendation system that suggests movies to users based on:
- Their own preferences.
- The preferences of similar users.

---

## **Algorithm Used**
The recommendation system is built using **SVD (Singular Value Decomposition)**:
- **SVD** is a matrix factorization technique widely used in collaborative filtering.
- It decomposes the user-item rating matrix into three smaller matrices, revealing **latent factors** that represent hidden patterns and preferences.
- These latent factors are used to predict how a user would rate movies they haven’t seen yet.

---

## **Key Steps**
### 1. **Data Loading and Preprocessing**
- The dataset consists of user ratings for Netflix movies.
- Steps include:
  - Reading the data.
  - Cleaning and filtering to remove:
    - Inactive users.
    - Movies with insufficient ratings.

### 2. **Model Building**
- The **Surprise library** is used to implement the SVD algorithm.
- The model is trained on a subset of the data to learn user preferences and movie patterns.

### 3. **Recommendation Generation**
- The system:
  1. Filters data to identify movies a specific user liked.
  2. Predicts ratings for all other movies for that user using the trained SVD model.
  3. Sorts the predictions to recommend the **top movies** with the highest predicted ratings.

---

## **Key Features**
- **Tools & Technologies:**
  - Python
  - Surprise Library (for SVD)
  - Pandas and NumPy (for data preprocessing)
  - Matplotlib (for visualization)
- **Performance Metrics:**
  - Evaluated the model using metrics like **RMSE (Root Mean Squared Error)**.
  - Achieved **optimized results** through parameter tuning and cross-validation.

---

## **How to Run the Project**
1. Clone the repository:
   ```bash
   git clone https://github.com/JADHAVRAJVARDHAN/Netflix-Movie-Recommendation-System.git
