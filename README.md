#Spotify Songs Genre Segmentation and Recommendation System
This project uses a Spotify dataset to group songs based on their audio features and to build a simple recommendation system similar to how Spotify suggests music.

#Project Summary
The goal of the project is to understand how songs are grouped using their characteristics and how these groups can be used to recommend similar tracks. The project includes data preprocessing, analysis, clustering and a basic recommendation function.

#Dataset Information

##The dataset contains:
track name
track artist
playlist genre
playlist name
audio features like danceability, energy, valence, loudness, tempo and others

#Categorical columns are converted into numerical values before modeling.

#Data Preprocessing
##Steps included:
Removing duplicate rows
Removing missing values
Label encoding the categorical columns
Scaling all numerical values using StandardScaler

#Exploratory Data Analysis

##The project includes:
Histograms for numeric columns
Boxplots to check for outliers
Counts of playlist genres
Counts of playlist names
Pairplots of important audio features
Correlation matrix for numerical features

#Clustering

Two clustering techniques were used.

##K-Means clustering
##Elbow method used to estimate number of clusters
#Silhouette score used to compare cluster quality
#Final clustering applied using the best cluster count

#Hierarchical clustering
Ward method used for linkage
Dendrogram plotted to visualize song grouping

#PCA
Two dimensional PCA used to display clusters on a scatter plot
Clusters visualized based on playlist genres and playlist names

#Recommendation System

A simple content based recommendation system was created using cosine similarity.
The function returns songs that are closest in terms of their audio features.

#Example:
recommend(10, top_n=5)

How to Run

#Install required packages:
pip install -r requirements.txt

#Run the script:
python spotify_clustering.py

#Place the dataset file spotify dataset.csv in the same folder.

#Technologies Used

Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
Scipy

#Future Work
Adding an interactive UI for recommendations
Using deep learning models for better embeddings
Including lyrics based features
Building a hybrid recommendation system

Author
@Anshika Garg
