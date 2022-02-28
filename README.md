# Sentiment Analysis of Yelp Reviews Dataset with CNN and LSTM
### Data Sourece
- Link : <https://www.kaggle.com/omkarsabnis/yelp-reviews-dataset>
### Data preprocessing
1. Map the value of stars between 0 and 1
2. Create word dictionary and convert sentence to word index.
    * build 25,000 tokens with vectorizer and convert original sentence to 300 Dimension sequence word list.
3. Convert text to vector using gloove.6b.300 pretrain model.
### Model
1. LSTM
    * Optimizer : Nadam
    * CUDNNLSTM
2. CNN
    * Optimizer : Nadam
### Evaluation
1. LSTM
    * Plot of Loss
    * Plot of Accuracy
    * Accuracy : 0.8035
2. CNN
    * Plot of Loss
    * Plot of Accuracy
    * Accuracy : 0.8365
