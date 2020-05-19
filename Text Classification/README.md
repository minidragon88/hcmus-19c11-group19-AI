# Overview
This is for solving The Text Classification

text_classification_CNN has implemented a classifier using CNN base on [Convolutional Neural Networks for Sentence Classification - Yoo Kim](https://www.cs.cmu.edu/~diyiy/docs/naacl16.pdf)

# Download Labeled train data and Pre-trained Glove Vector (if needed)
```
# download imdb train from Kaggle in the below link and keep the files in the working directory
https://www.kaggle.com/c/word2vec-nlp-tutorial/download/labeledTrainData.tsv
# download glove word vector
wget http://nlp.stanford.edu/data/glove.6B.zip
unzip glove.6B.zip
```

# Run text_classification_CNN in Google Colab
1) Modify the path to your Google Drive 
* *TSV_DIR* is the location of *labeledTrainData.tsv*
* *GLOVE_DIR* is the location of *Glove 6B 100d*

2) Run the **Prepare dependencies and global variables** block to load dependencies and prepare variables

3) Run the **Prepare dependent functions** block to load all functions needed

4) Run **Prepare data to train** to prepare the data to train

The implementation contains 2 different approach
* A simplified convolutional approach which use total 128 filters with size 5 and max pooling of 5 and 35
* A Deeper Convolutional neural network which is implemented in Yoon Kim’s paper, applying multiple filters.

You can use either of them to compare the difference in accuracy
