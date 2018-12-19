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

## Collaborative Filtering (Model 2)
- Can select Data-set size
- n_similar user/items can be selected to choose how many similar users or items to be used to make prediction
- Functionality added to save predictions as 'user-user-predictions.npy' and 'item-item-predictions.npy' that contain all the predictions made for user-joke pairing.
- Code reports the MAE for test set. Validation split set to 0.1 right now, but that can be changed.
- Added functionality to sort prediction matrix mentioned earlier, and get a new matrix where each row corresponds to jokes recommended to the user. The leftmost value is the most desirable. The files are saved as 'item-item-cf-sorted.npy' and 'user-user-cf-sorted.npy'.
- Added functionality to display top-n jokes for a certain user.
