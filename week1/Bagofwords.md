# # Bag of words for multilabel classification

This notebook will use LSTM to do NER analysis. 

**Data** contains tweets dataset of post titles from StackOverflow with correspoding tags.

**Bag of words**  it is a sparse word matrix representation for a text. In this notebook 5000 most frequent words were in the representation.
If word appeared in the post title it got value increased by one for the column on position of that specific word in bag of words model. 
Counts were processed with TF-IDF technique that penalises too frequent words and provides better features space.


