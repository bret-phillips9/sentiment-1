This project produces a Quarto document that ingests a CSV file of tweets that have been labeled as possessing either good, bad, or neutral sentiment towards ChatGPT.  

The text of each tweet is converted into embeddings by (ironically) ChatGPT.

The embeddings data are split into training and test sets.

The training set embeddings are used to train a resampled GLM with 10-fold cross-validation.

The resulting model weights are then applied to the test set embeddings and evaluated via a confusion matrix.
