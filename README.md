# Sentiment-Analysis with LSTM and GRU

Applying deep learning techniques to the NLP task of Sentiment analysis. Here, we are determining the text's emotional tone is positive(1) 
or negative(0) on Imdb review dataset with the help of Keras and Tensorflow.

After importing the libraries, I have embedded the review texts using word embeddings(vector representation of a word) , by embedding layers
in keras. After the embedding layer, I have added a LSTM layer with 128 units and a dropout of 0.2 for regularization and then added a dense
layer with sigmoid activation function to give the output of 0(negative) or 1(positive). The loss function used is binary_crossentropy and
optimizer is rmsprop. With this simple keras model, I could achieve a accuracy of 87%.
I have also tried CuDNNLSTM and CuDNNGRU which trains much faster using GPUs and yields good accuracy.
