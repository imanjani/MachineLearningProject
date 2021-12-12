# Machine Learning Projects



#### 1  Categories of clustering algorithms

The algorithms we use fall into three different categories:

* Centroid-based clustering
* Density-based clustering
* Hierarchical clustering

The algorithms used in the Notebook are as follows:

| Category | Algorithm | Description |
| --- | --- | --- |
| Centroid-based | k-means | Find a predetermined number (k) of center points to create k clusters based on distance from center. |
| Centroid-based | mean shift | Seek areas of higher density to determine cluster centers. |
| Density-based | DBSCAN | Separate out the noise (points in sparse regions) and group together data in dense regions. |
| Hierarchical | agglomerative clustering | Start with each point as its own cluster and then merge the nearest cluster until the goal is reached. |

<img src="https://github.com/imanjani/Machine_Learning_Projects/blob/master/data/clustering3D.gif">

---

#### 2 - Forecasting-Bitcoin-Prices (ARIMA, XGBoost, Prophet, LSTM)
Forecasting Bitcoin Prices via ARIMA, XGBoost, Prophet, and LSTM models in Python.
Description: In this repo, I will test the Bitcoin forecasting abilities of 4 different Machine Learning models in Python: ARIMA, Prophet, XGBoost, and LSTM. By splitting the data into a testing and training set, I will compare each model’s performance with one another and conclude which performed best.

<img src="https://media.giphy.com/media/8yQady2pFVfGJSnde7/giphy-downsized.gif">



---

#### 3 - Stacking Model

Using Model-Stacking to boost model performance and accuracy

<img src="/Stacking Model/Data/1.jpeg" width="60%" >

---



#### 4 - Recommendation Engine with Python (Movie Recommendations)
  - SVD Matrix Factorization
  This method involves embedding movies in a vector space by using a stochastic estimation of Matrix Factorisation. The movie embedding can be considered a representation of the movie features and we can make recommendations using a similarity metric.
  
  - Content-Based and Collaborative Filtering (CF)
   Collaborative filtering (CF) is more commonly used than content-based systems because it usually gives better results and is relatively easy to understand (from an overall implementation perspective). The algorithm has the ability to do feature learning on its own, which means that it can start to learn for itself what features to use.
   CF can be divided into Memory-Based Collaborative Filtering and Model-Based Collaborative filtering.
   Here, I will implement Model-Based CF by using singular value decomposition (SVD) and Memory-Based CF by computing cosine similarity.
