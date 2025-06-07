# 🎧 Spotify Mood Playlist Clustering using K-Means (from Scratch)

## 📌 Motivation

With millions of tracks available on streaming platforms like Spotify, users often struggle to discover songs that match their mood or activity. Can we build a system that clusters music based on emotional "vibe" using only audio features?

This project explores how **unsupervised learning** — specifically **K-Means clustering** — can be used to automatically group songs into **mood-based playlists**, without any labeled data.

---

## 🎯 Objective

To build a mood-based playlist recommendation engine by:

- Clustering songs using audio features like **energy, danceability, valence, tempo**, etc.
- Implementing **K-Means from scratch** (no built-in ML libraries like `sklearn`)
- Interpreting clusters based on mood and use-cases for **automated playlist creation**

---

## 🎶 Why Spotify?

- 🎵 **80+ million tracks** are available for streaming
- 🧠 Music plays a major role in regulating mood, focus, and productivity
- 🎯 Listeners often seek **vibe-based playlists** (e.g., chill, workout, party)
- 📊 Spotify provides rich **numerical audio features** suitable for clustering

---

## 🔄 Project Flow

1. 📁 **Data Collection**  
   Dataset of ~10,000 Spotify tracks with features from Kaggle

2. 📊 **EDA & Visualization**  
   - Distribution plots of loudness, energy, acousticness, etc.  
   - Correlation heatmap to explore relationships

3. ⚖️ **Feature Scaling**  
   - Standardized features to avoid bias in clustering  
   - Used MinMax or Z-score scaling

4. 💡 **Elbow Method**  
   - Plotted inertia to determine optimal `k`  
   - Identified the "elbow" point

5. 🔁 **K-Means Clustering (from Scratch)**  
   - Random centroid initialization  
   - Assignment based on Euclidean distance  
   - Iterative update of centroids until convergence

6. 🎨 **Cluster Visualization**  
   - 2D plots (PCA-reduced) showing mood clusters  
   - Compared high-energy/danceable vs. low-tempo/acoustic songs

7. 💡 **Business Use Case**  
   - Each cluster = mood-based playlist  
   - Potential application in **automated playlist generation** for music apps

---

## 🧠 Key Learnings

- Understood how **unsupervised learning** works without labels
- Learned **K-Means algorithm internals** — from centroid logic to convergence
- Discovered the importance of **feature scaling and distance metrics**
- Connected ML logic to real-world business applications in music discovery

---

## 🛠️ Tools & Libraries

- Python 🐍  
- NumPy  
- Pandas  
- Matplotlib  
- Seaborn

---

## 📸 Visuals (Add These to Boost Appeal)

> You can upload these in an `images/` folder and reference them below:

| Step | Image Suggestion | Markdown Example |
|------|------------------|------------------|
| **Mood Mapping** | A diagram like [Spotify mood energy map](https://research.atspotify.com/files/ACM_RecSys_2017_The_Mood_of_Music.pdf) | `![Mood Map](images/mood_map.png)` |
| **Elbow Method** | Your inertia vs. k plot | `![Elbow](images/elbow_plot.png)` |
| **K-Means Visual** | PCA-reduced cluster plot | `![Clusters](images/kmeans_clusters.png)` |
| **Business Insight** | Icons showing playlists like "Party", "Chill", "Focus" | `![Playlists](images/mood_playlists.png)` |

---

## 📁 Folder Structure

