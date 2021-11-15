# Recommendation Engine with Python
creating a recommendation system with Python using Movie Lens Data Set.
___

## 1.Collaborative Filtering
Collaborative filtering produces recommendations based on the knowledge of users’ attitude to items, that is it uses the "wisdom of the crowd" to recommend items. 

In general, Collaborative filtering (CF) is more commonly used than content-based systems because it usually gives better results and is relatively easy to understand (from an overall implementation perspective). The algorithm has the ability to do feature learning on its own, which means that it can start to learn for itself what features to use. 

CF can be divided into **Memory-Based Collaborative Filtering** and **Model-Based Collaborative filtering**. 

Here, I will implement Model-Based CF by using singular value decomposition (SVD) and Memory-Based CF by computing cosine similarity. 


## 2.SVD Matrix Factorization
SVD Matrix Factorization This method involves embedding movies in a vector space by using a stochastic estimation of Matrix Factorisation. The movie embedding can be considered a representation of the movie features and we can make recommendations using a similarity metric.
