# Data Analytics Project
## Movie Recommendation System

### Description
* We have taken the movielens dataset, which is available in kaggle:
	* https://www.kaggle.com/rounakbanik/the-movies-dataset 
	* https://www.kaggle.com/carolzhangdc/imdb-5000-movie-dataset
	* https://drive.google.com/drive/folders/1of45AVydAAaDwvQIZWl6Pyj8BkRx8IVM?usp=sharing (Here's the drive link for the entire dataset for our project)
	
* After pre-processing, for designing the **Model** we have saved the dataset in https://drive.google.com/drive/folders/1of45AVydAAaDwvQIZWl6Pyj8BkRx8IVM?usp=sharing over here.

* The codes for pre-processing of the dataset are present in preprocess1.ipynb and preprocess2.ipynb file.

* The file Recommendation_CosineSimilarity.ipynb contains the model implementation for Recommendation System using **Cosine Similarity**, which is an **Content-Based Filtering technique**. 


* The file collaborative_filtering_surprise.ipynb contains the model implementation for Recommendation System using **KNN**, which is an **Collaborative-Based Filtering technique**. 

### Model Implemention

* **Recommendation using Cosine Similarity :**

	It is Content-based filtering technique, wherein we would be finding the similarities between the two vectors (two different rows from the dataset) by applying the cosine of two vectors. Here, as per our data, we use the cast, genre and the keywords (plot of the movie) and cascade them as a single text and use the infamous Tf - Idf transformation to convert the text to vector for further vector calculations.

* **Recommendation using KNN :**
	
	KNN falls under the supervised algorithms. We make use of this approach and the data containing the users and their movie ratings. The estimated rating is basically a weighted mean of the ratings the user gave to familar items, weighted by the similarities.
	
	We have used Surprise library for this implementation, which is an Python scikit for Recommendation System.
