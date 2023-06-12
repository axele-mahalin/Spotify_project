# Spotify recommender

# Description

My project aims to recommend songs using the Spotify API based on a song given by a user.
I used an unsupervised machine learning model.

# Planning

- Cluster the songs I collected
- Scale the audio features of the songs and store the scaler
- Initialize a KMeans model 
- Fit the model sing kmeans.fit(X_scaled)
- Predict the cluster using X["cluster"] = kmeans.predict(input_song)
- Create a user interface so that the user can gives a song as input

# Project pipeline:

When the user inputs a song (let’s imagine it’s Bohemian Rhapsody):
- it sends “Bohemian Rhapsody” to the Spotify API and get its audio features
- store them in a variable called, scale the audio features, get the cluster of the song (let’s imagine it’s cluster 3)
- from the songs I collected, get a random song that belongs to cluster 3. (let’s imagine it’s Stairway to Heaven)
- print Stairway to Heaven: this is the recommendation!

The Input_user.ipynb has to be used for the user interface.
