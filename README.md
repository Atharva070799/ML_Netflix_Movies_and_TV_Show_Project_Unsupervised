# NETFLIX_MOVIES_AND_TV_SHOWS_CLUSTERING
This project clusters Netflix movies and TV shows based on attributes like ratings, genres, and release years. It helps users find similar content and provides insights for content creators. Python code includes data preprocessing, feature engineering, model selection, and evaluation.

![image](https://github.com/Shraddha6999/NETFLIX_MOVIES_AND_TV_SHOWS_CLUSTERING/assets/123643720/72f28a29-a302-4a14-b774-2a51da4c3009)


![image](https://github.com/Shraddha6999/NETFLIX_MOVIES_AND_TV_SHOWS_CLUSTERING/assets/123643720/13f1d989-c909-4b38-aca7-0c0ae4d64fd4)

## Overview
Netflix is a subscription-based streaming service that provides its members with access to a vast library of movies and TV shows. With such a large content catalog, it can be challenging for users to find content that matches their preferences. To address this issue, Netflix uses data analysis and machine learning techniques such as clustering to group their content into similar categories. This repository focuses on the data-driven approach of clustering Netflix's movies and TV shows to improve the user experience and provide personalized recommendations.

## Objective
The primary objective of Netflix Movies and TV Shows Clustering is to enhance the user experience on Netflix by providing personalized content recommendations based on viewers' preferences and viewing history. By organizing the content library into clusters, Netflix aims to suggest titles that are more likely to match user interests, resulting in increased user engagement, satisfaction, and ultimately, improved retention and revenue for the company.

## Dataset
Netflix_movies_and_series_dataset_link:- https://drive.google.com/file/d/1EuTT5bkkO1kdgVuih1tsBrOhS1ya5OjY/view?usp=sharing

**show_id** : Unique ID for every Movie / Tv Show

**type** : Identifier - A Movie or TV Show

**title** : Title of the Movie / Tv Show

**director** : Director of the Movie

**cast** : Actors involved in the movie / show

**country** : Country where the movie / show was produced

**date_added** : Date it was added on Netflix

**release_year** : Actual Releaseyear of the movie / show

**rating** : TV Rating of the movie / show

**duration** : Total Duration - in minutes or number of seasons

**listed_in** : Genere

**description** : The Summary description

## Conclusion
**CONCLUSION FROM EDA:**

1) Netflix has more movies than TV shows available on the platform.

2) The majority of content on Netflix is suitable for mature audiences, with a TV-MA rating being the most common.

3) The United States is the country with the highest number of productions available on Netflix, followed by India and the United Kingdom.

4) Netflix has seen a steady increase in its content library since its inception in 2008.

5) The most common genre of content on Netflix is Dramas, followed by Comedies and Documentries.

6) The Wordcloud visualization of movie descriptions shows that some of the most common words used in Netflix movie descriptions include love, family, young, life, and world.

7) The correlation heatmap shows that there is a moderate positive correlation between the duration of a movie and its release year.

8) The pairplot shows some interesting patterns between variables such as the strong positive correlation between the number of reviews and the year of release, as well as a negative correlation between the rating and duration of a movie.

**CONCLUSION FROM MODEL IMPLEMENTATION:**

1) The data was clustered based on the attributes: director, cast, country, genre, rating, and description.

2) TFIDF vectorizer was used to tokenize, preprocess, and vectorize the values in these attributes, creating a total of 20000 attributes.

3) Principal Component Analysis (PCA) was used to reduce the dimensionality of the data which captured more than 90% of the variance.

4) **K-Means Clustering** algorithm was used to build clusters with the optimal number of clusters being **6** based on the elbow method and Silhouette score analysis.

5) **Agglomerative clustering** algorithm was used to build clusters with the optimal number of clusters being **9** based on the dendrogram visualization.

6) A content-based **recommender system** was built using cosine similarity and will make 10 recommendations to the user based on the type of show they watched.

7) **DBSCAN clustering** was built and it gives optimal number of clusters as 21 with very less metric score.

## Clustering Process
The clustering process involves analyzing various data points, including genre, cast, director, plot, and other relevant features, to identify patterns and similarities between different titles. Netflix employs unsupervised machine learning algorithms such as k-means, hierarchical clustering, and principal component analysis (PCA) to group movies and TV shows with similar features into distinct clusters or categories.
The algorithms work as follows:

- **K-means**: This algorithm partitions the data into k clusters, where k is predefined. It iteratively assigns data points to the nearest centroid and adjusts the centroid positions based on the assigned points. K-means is effective for clustering movies and TV shows with similar features into distinct groups representing unique genres or categories.
- **Hierarchical Clustering**: This technique creates a tree-like structure that organizes movies and TV shows into similar categories based on their characteristics. It starts with each title as a separate cluster and iteratively merges clusters based on their similarity, forming a hierarchical structure.

## Benefits
Clustering is a powerful tool that enables Netflix to analyze and group its vast library of content into similar categories, providing users with personalized recommendations and improving the overall user experience. Some key benefits of clustering include:
1. **Personalized Recommendations**: By leveraging clustering techniques and analyzing users' viewing history and preferences, Netflix can recommend content that aligns with their interests. This personalized approach increases user engagement, satisfaction, and the likelihood of users continuing their subscriptions.
2. **Data-Driven Decision Making**: Clustering enables Netflix to make informed decisions about content production and licensing. By understanding underlying trends and patterns in user behavior, the platform can optimize its content library, produce or acquire titles that resonate with its user base, and remove those that are less successful.

## Repository Structure
This repository contains the following files and directories:
- **data**: This directory stores the dataset used for clustering Netflix movies and TV shows. It includes relevant features such as genre, cast, director, and plot.
- **notebooks**: This directory contains Jupyter notebooks that demonstrate the clustering process and analysis step-by-step. It includes detailed explanations of the algorithms used and their implementation.
- **results**: This directory holds the clustering results, such as the grouped clusters and their corresponding titles. It also includes any visualizations or insights derived from the clustering analysis.
- **README.md**: This file provides an overview of the repository, its objectives, the clustering process, benefits, and repository structure.

## Usage
To use this repository, follow these steps:
1. Clone the repository to your local machine using the following command:
   ```
   git clone https://github.com/Atharva070799/ML_Project_Unsupervised/edit/main/README.md
   ```
2. Navigate to the `notebooks` directory and open the Jupyter notebooks to explore the clustering process, algorithms, and analysis.
3. Access the `data` directory to retrieve the dataset used for clustering
