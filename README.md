# Collaborative_Recommender_RBM
This implmentation of Python shows the usage of a Restricted Boltzmann Machine (RBM) in a Collaborative Filtering based recommendation system. This system is an algorithm that recommends items by trying to find users that are similar to each other based on their item ratings. The Model is built using tensorflow, numpy and pandas. Our model of the RBM has two layers of neurons, one is the visible input layer and the other is a hidden layer. The hiddenlayer is used to learn features from the data fed though the input layer. We train the RBM on the input data and have the hidden layer learn its features. These features are then used to recontruct the input, which in our case, will predict the ratings(i.e probability that the user will like the movie) for movies that the particular user has not seen. In this way we can recommend.

Requirements:
1. Tensorflow v1.3 or above.
2. Numpy
3. Pandas
4. MatPlotLib

Steps:
1. Load in the movies and ratings datasets
2. Format and merge the data
3. Build model placeholders and set parameters, error functions and update methods (we use sigmoid and relu for activation)
4. Initialize variables
5. Train the RBM and plot progress
6. Make predictions by feeding in a particular userID and reconstruct input probabilities
7. Remove already watched movies and recommend to the user

All steps have been described and implemented in the Jupyter Notebook

Reference Links: 
1. https://medium.com/@m_n_malaeb/the-easy-guide-for-building-python-collaborative-filtering-recommendation-system-in-2017-d2736d2e92a8
2. https://cambridgespark.com/content/tutorials/implementing-your-own-recommender-systems-in-Python/index.html
3. http://www.data-mania.com/blog/recommendation-system-python/
4. https://www.analyticsvidhya.com/blog/2016/06/quick-guide-build-recommendation-engine-python/
5. http://dataaspirant.com/2015/05/25/collaborative-filtering-recommendation-engine-implementation-in-python/
6. https://getstream.io/blog/factorization-machines-recommendation-systems/

Research Papers:
1. http://www.machinelearning.org/proceedings/icml2007/papers/407.pdf - Restricted Boltzmann Machines
for Collaborative Filtering, Hinton et. al.
2. https://arxiv.org/pdf/1606.07129.pdf - Explainable Restricted Boltzmann Machines for Collaborative
Filtering - Nasraoui
