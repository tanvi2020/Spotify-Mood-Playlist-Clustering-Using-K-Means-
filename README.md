# Spotify-Mood-Playlist-Clustering-Using-K-Means-

This project started with a simple idea: Can we group songs into mood-based playlists using their audio features? I used a Spotify tracks dataset from Kaggle, which contains details like energy, danceability, tempo, valence, and more for a bunch of songs. The goal was to cluster these songs into different moods or vibes — all without using any built-in machine learning libraries.

I began by cleaning and exploring the dataset. Luckily, there weren’t any missing values, so I could dive straight into analyzing the features. I used visualizations to understand how different attributes like loudness, acousticness, and tempo are spread across the songs. Since clustering is sensitive to feature scale, I made sure to scale all the numeric features before building the model.

The core part of the project was implementing the K-Means algorithm completely from scratch — no scikit-learn, just NumPy and logic. I first used the Elbow Method to figure out how many clusters would make sense. Then I randomly initialized centroids, assigned each song to the nearest one using Euclidean distance, and updated the centroids based on the mean of the points in each cluster. This process repeated until the centroids stopped moving — that’s when I knew the clustering had stabilized.

Once the clusters were formed, I plotted the results and started interpreting them. Some clusters had high energy and danceability, while others leaned more towards acoustic and low-tempo tracks — this made it clear how K-Means was grouping songs based on their audio mood. It was interesting to see how well the algorithm could capture the essence of different types of music just from numbers.

This project helped me understand how unsupervised learning works and especially how K-Means learns structure from unlabelled data. More than just running code, building the algorithm myself gave me a much deeper grasp of concepts like centroid movement, distance calculation, and convergence. It also showed how clustering can be applied in real-world scenarios like music recommendation and playlist generation.

# Tools Used
- Python 🐍
- NumPy
- Pandas
- Matplotlib
- Seaborn
