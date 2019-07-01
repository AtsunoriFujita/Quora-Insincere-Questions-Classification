# Quora Insincere Questions Classification

This respository contains my code for competition in kaggle.


53rd Place Solution for [Quora Insincere Questions Classification](https://www.kaggle.com/c/quora-insincere-questions-classification "Quora Insincere Questions Classification")


### Model
- Based on Recurrent Convolutional Neural Network. I referred to this [repository](https://github.com/AnubhavGupta3377/Text-Classification-Models-Pytorch/tree/master/Model_RCNN)
- Word embeddings use glove, paragram, word2vec, fasttext. And applied PCA(1200 → 300)
- LSTM + GRU + Self Attention + Max pooling
- Loss function: FocalLoss
- Optimizer: AdamW

### train
- n_splits = 4
- batch_size = 2048
- train_epochs = 5
- base_lr, max_lr = 0.001, 0.003  
- Weight Decay = 0.0001
- Learning schedule: CyclicLR


Public score: 0.69768    
Private score: 0.70532
