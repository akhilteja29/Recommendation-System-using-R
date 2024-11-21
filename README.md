This R script builds a movie recommendation engine using an **Item-Based Collaborative Filtering (IBCF)** approach. It utilizes data from IMDb, including movie details (e.g., genres, titles) and user ratings. The key steps include:

1. **Data Preprocessing**: The script starts by loading and processing the movie and rating data, creating a one-hot encoded matrix for movie genres, and constructing a search matrix for easy genre-based queries.
   
2. **Matrix Creation**: It transforms the rating data into a **realRatingMatrix**, a data structure suitable for building recommendation models in R.

3. **Similarity Calculation**: The script computes similarity matrices both for **users** and **items** (movies) using cosine similarity, and visualizes these similarities using heatmaps.

4. **Data Exploration**: Visualizations are created to analyze the distribution of movie ratings, the most viewed movies, and user behaviors (e.g., average ratings per user).

5. **Recommendation Model**: It splits the data into training and testing sets, builds an IBCF recommendation model using the `recommenderlab` package, and evaluates the model's performance by predicting movie recommendations for users.

6. **Prediction and Evaluation**: The model predicts top movie recommendations for each user, and the results are displayed as movie titles. Further analysis is performed to examine the distribution of recommended items across users.

The entire process is visualized through various plots, including heatmaps, bar plots, and distribution charts, to gain insights into movie recommendations, user preferences, and the behavior of the recommendation system.