# # Recognise named entities on Twitter with LSTMs

This notebook will use LSTM to do NER analysis. 

**Data** contains tweets with NER tags. Every line of a file contains a pair of a token (word/punctuation symbol) and a tag, separated by a whitespace. Different tweets are separated by an empty line.

**LSTM**  we feed the model with embedding variable for all the words(tokens) in tweets. Embedding matrix is at first randomly initialised and during the training it is updated to produce the best embeddings for each token that can help with NER. 
\
The lookup function is used to retrieve the rows that embed all the words in each sample of input batch. 
Lets say size of batch is 32. Each of the 32 samples is a tweet with n words. Each word is embedded with a vector of dimension d. Each sample will then be represented with embedding of shape [n,d]. 
