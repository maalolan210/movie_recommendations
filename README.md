# movie_recommendations
CSE 368 final project

**DESCRIPTION:**

In this project our objective is to build a linear regression based
machine learning model that predicts the relationship between
movie titles and their rating with their respective genres, in order
to offer shows of similar recommendation.

Movie or content recommendations have quickly become very
common applications of allowing users to source different
interests of whatever media that they’re watching & enjoying.

Huge streaming giants such as Netflix or Hulu actively use these
type of recommendations. Amazon’s “frequently bought together”
feature also involves similar recommendation system like the
we’ve implemented.


**BACKGROUND:**
We’ve used linear regression that we learned
in this class to reproduce movie/show
recommendations. The role of linear
regression in movie recommendation
systems and our project, as well as in other
recommendation platforms, is the ability to
predict ratings or common genre shows.

The algorithm we used employs a linear model to
fit a line to the data that represents the
relationship between the features of the movies
and their ratings. The model is trained on a dataset
of movies and their ratings, and then used to
predict the ratings for movies that are in the
training dataset.

**IMPLEMENTATION:**

In order to extract info from our dataset, which in this case is the IMDB movies database, we load the data
set within our program using Pandas. This dataset contains a plethora of information about movies,
including their titles, genres, ratings, and other metadata. To build the recommendation system, we look
to see ratings for movies within specific genres in order to predict related movies with similar ratings that
are within the same genres.

After extraction of the data from the IMDB set, we split the dataset into a training set and a test set. With the
training sets purpose being to train the model itself, we adjust the model using the split set parameters to
minimize potential errors between predicted ratings and actual ratings within the training set.

Now we train the linear regression model on the dataset itself. The predicted rating is a value between 1 and 10 that represents the model's estimate of
how the movie will be rated by users.

Using the value, we are able to get recommend a set
of movies within the same genre with similarly
predicted ratings. This allows a compilation of
movies that users may enjoy.

To do this the relevant characteristics such as genre
and rating in relation to other movies of similar genres
were used to create a rating prediction.

**FUTURE DEVELOPMENT:**

In order to train for even
100 iterations our
computer (Macbook) is not
powerful enough to do so
in a reasonable amount of
time.

Implementing gradient descent
and tuning parameters such as
Learning Rate, Gamma, or
number of iterations to name a
few to increase model training
performance.

Use a different type of
Linear Regression model
for faster and more
efficient training such as
SGDRegression (Stochastic
Gradient Descent)
