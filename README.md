# Sentiment Analysis of Yelp Reviews Dataset with CNN and LSTM
### Data Sourece
- Link : <https://www.kaggle.com/omkarsabnis/yelp-reviews-dataset>
### Data preprocessing
1. Map the value of stars between 0 and 1
2. Create word dictionary and convert sentence to word index.
    * build 25,000 tokens with vectorizer and convert original sentence to 300 Dimension sequence word list.
    
    ![imgae](https://github.com/KartaYu/Sentiment-Analysis-of-Yelp-Reviews-Dataset-with-CNN-and-LSTM/blob/main/Pic/word%20dictionary.png)
3. Convert text to vector using gloove.6b.300 pretrain model.
    ![imgae](https://github.com/KartaYu/Sentiment-Analysis-of-Yelp-Reviews-Dataset-with-CNN-and-LSTM/blob/main/Pic/vector%20model.png)
### Model
1. LSTM
    * Optimizer : Nadam
    * CUDNNLSTM
    
    ![imgae](https://github.com/KartaYu/Sentiment-Analysis-of-Yelp-Reviews-Dataset-with-CNN-and-LSTM/blob/main/Pic/LSTM.png)
2. CNN
    * Optimizer : Nadam
    
    ![imgae](https://github.com/KartaYu/Sentiment-Analysis-of-Yelp-Reviews-Dataset-with-CNN-and-LSTM/blob/main/Pic/CNN.png)
### Evaluation
1. LSTM
    * Plot of Loss
    
    ![imgae](https://github.com/KartaYu/Sentiment-Analysis-of-Yelp-Reviews-Dataset-with-CNN-and-LSTM/blob/main/Pic/loss%20of%20lstm.png)
    * Plot of Accuracy
    
    ![imgae](https://github.com/KartaYu/Sentiment-Analysis-of-Yelp-Reviews-Dataset-with-CNN-and-LSTM/blob/main/Pic/acc%20of%20lstm.png)
    * Accuracy : **0.8035**
2. CNN
    * Plot of Loss
    
    ![imgae](https://github.com/KartaYu/Sentiment-Analysis-of-Yelp-Reviews-Dataset-with-CNN-and-LSTM/blob/main/Pic/loss%20of%20cnn.png)
    * Plot of Accuracy
    
    ![imgae](https://github.com/KartaYu/Sentiment-Analysis-of-Yelp-Reviews-Dataset-with-CNN-and-LSTM/blob/main/Pic/acc%20of%20cnn.png)
    * Accuracy : **0.8365**
