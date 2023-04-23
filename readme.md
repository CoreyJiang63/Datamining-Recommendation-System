Our code directory consists of the following files:

- Preprocessing.ipynb: We do preprocessing on our dataset in this file, as well as visualization to provide the reader with an insight into our problem settings and the data we use.
- Basline.ipynb: We use the preprocessed data to build our baseline model using `Surprise` package. The baseline system cannot always submit the "top-10" recommendations, as our feature space is quite sparse, and we do not have sufficient information to recommend 10 items.
- proximity_matrix.ipynb: We use our preprocessed reviews data to build user-item proximity matrix (interactions), and we use it to build LightFM model for recommendation.
- approx_svd.ipynb: We use approximate SVD to further improve our model's performance and efficiency. We can reduce the dimensionality of the matrix by identifying the most important features, or latent factors, that capture the underlying patterns in the user-item interactions. After recommendation, we project the recommendation space into 2-dimensional space using methods similar to PCA, and visualize our result.