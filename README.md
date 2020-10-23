# Movie Recommendation System

Dataset: https://grouplens.org/datasets/movielens/latest/


## EDA

Fortunately, the Movielens dataset was very clean. For my early analysis I looked at the ratings and genres to understand how they were distributed in my dataset.

![Image]('ratings.png')

![Image]('genres.png')


## Building Recommendation System

1. Simple recommendation system 
2. Collaborative filtering 
    a. memory-based: item-to-item and user-to-user
    c. model-based: SVD and KNNs
3. Content-based filtering 
4. Evaluation of models


## Conclusion and Future Steps

To evaluate my collaborative filtering models, I looked at the RMSE score. RMSE measures the difference between values predicted by the model and the values observed, therefore, the lower our RMSE score the better our model is performing. Our SVD model performed the best with an RMSE score of 0.86.

One future step for me would be to combine my SVD and content-based model to build a hybrid model. A hybrid model combines collaborative and content-based filtering to utilize their advantages and address their disadvantages. A hybrid model can help with addressing issues such as the cold start problem or popularity bias. I would first used content-based filtering to receive recommendations and then sort through these recommendations using the SVD model. It is important to note that in building a hybrid model, it can be difficult to find the right balance between the two approaches. 

Another future step would be to do some more empirical testing with personally known individuals as another measure of performance.

Lastly, I would want to test my models across different use cases to ensure it will be compatible with various streaming platforms.
