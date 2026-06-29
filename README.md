# 🎵 Spotify Music Recommendation System using Machine Learning

A **Content-Based Music Recommendation System** that groups similar songs using **Unsupervised Machine Learning** and recommends songs based on their audio characteristics using **Cosine Similarity**.

---

## 📌 Project Overview

Music streaming platforms contain millions of songs, making it difficult for users to discover music that matches their preferences. This project builds a **Content-Based Recommendation System** by analyzing Spotify audio features, clustering similar songs using **K-Means Clustering**, and recommending songs with similar characteristics using **Cosine Similarity**.

The project demonstrates the application of **Machine Learning**, **Data Analysis**, and **Recommendation Systems** to solve a real-world problem.

---

## 🎯 Problem Statement

Traditional music search relies on users knowing the exact song or artist they want to listen to. However, discovering similar songs based on musical characteristics is challenging.

The objective of this project is to automatically identify similar songs using their audio features and provide personalized song recommendations.

---

## 🚀 Project Workflow

```
📂 Dataset
      ↓
🧹 Preprocessing
      ↓
📊 Exploratory Data Analysis (EDA)
      ↓
⚖️ Feature Scaling
      ↓
🤖 K-Means Clustering
      ↓
📈 Elbow Method & Silhouette Score
      ↓
📉 PCA Visualization
      ↓
📋 Cluster Profiling
      ↓
📐 Cosine Similarity
      ↓
🎵 Recommendation System
      ↓
✅ Top-N Song Recommendations
```

---

## 📊 Dataset

The project uses a Spotify songs dataset containing various audio features, including:

* Danceability
* Energy
* Loudness
* Speechiness
* Acousticness
* Instrumentalness
* Liveness
* Valence
* Tempo
* Popularity
* Duration

---

## ⚙️ Data Preprocessing

* Removed unnecessary columns
* Selected relevant numerical features
* Standardized features using **StandardScaler**
---

## 🔍 Exploratory Data Analysis

* Checked missing values and data types
* Analyzed feature distributions
* Generated correlation heatmap
* Identified relationships between important audio features

---

## 🤖 Clustering Algorithms

The following clustering algorithms were implemented and compared:

### ✔️ K-Means Clustering

* Elbow Method
* Silhouette Score
* PCA Visualization
* Cluster Profiling

### ✔️ DBSCAN

* Density-based clustering
* Compared using Silhouette Score

### ✔️ Hierarchical Clustering

* Dendrogram Analysis
* Compared using Silhouette Score

---

## 📈 Model Comparison

| Algorithm    | Evaluation Metric (Silhoutte Score)|
| ------------ | ------------------------ |
| K-Means      | **0.1868**               |
| DBSCAN       | 0.1395                   |
| Hierarchical | -0.1170                  |

**Final Model Selected:** **K-Means Clustering** which gives highest Silhoutte scores among all the models

---

## 🎵 Content-Based Recommendation System

The recommendation system was built using:

* Cosine Similarity
* Cluster-based filtering
* Top-N similar song recommendations

Recommendations are generated only from songs belonging to the same cluster, improving both recommendation quality and computational efficiency.

---

## 📊 Results

* Successfully grouped songs into meaningful clusters.
* Identified cluster characteristics using cluster profiling.
* Generated relevant song recommendations based on audio feature similarity.
* Demonstrated the effectiveness of combining clustering with cosine similarity for music recommendation.

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* PCA
* K-Means
* DBSCAN
* Hierarchical Clustering
