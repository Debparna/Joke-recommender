# JokeRecommendor
## Datasets used
- Jester-data-1
- Jester-data-2
- Jester-data-3
- JokeText.csv


## Neural-Network (Model 1 )
- Trained Model available for fulldata-set. Can make a trained model for a smaller dataset if needed. Let me know if a new model is needed since training is computationally heavy.

- Numba library is used to improve computation speed. Comment the import to the library, and "@jits" in code to not use Numba.

- Code outputs a file called UserJokeRating which contains the recommended jokes in order from left to right. Each row corresponds to a user, and every column contains the jth recommended joke. (Ex: Row0, Col0, contains the first joke recommended for user 1. NOTE: PYTHON INDEXES FROM 0)

- Prediction matrix is stored as predictions.npy. Code contains functionality to save the predictions. This is a user-joke matrix where the values are the ratings predicted.
