# Machine Translation 
## Bi-directional LSTM Attention Model 
 
The goal of this project is to first understand the mechanisms applied to construct an attention model by creating a machine translation model, which is able to recognize human-readable dates and translate them to machine-readable dates. This project is part of the labs offered in the course [Sequence Learning](https://www.coursera.org/learn/nlp-sequence-models ) by DeepLearning.ai. More explanation on the structure of the model can be found [here](Machine_translation.ipynb/). The attention model built is based on the paper by [Bahdanau et al., 2014](https://doi.org/10.48550/arXiv.1409.0473). 

Furthermore, the file [nmt_utils.py](nmt_utils.py/) creates the arbitary human-readable dates to train the model with. Some notes on how the additive attention mechanism works is also added: [Notes](Notes.pdf)

We will then apply the attention procedure to train a sentiment analysis model based on two datasets: 
- [Canva_reviews.xlsx](Canva_reviews.xlsx/): 

This dataset contains 1500 customer feedbacks for the app Canva and is part of the project "Build Multi Class Text Classification Models with RNN and LSTM" from [ProjectPro](https://www.projectpro.io/). We will use two embeddings for words one with one-hot vectors and another with GloVe embeddings. To check the resutls please check the file (Additiveattn+1125data.ipynb)[Additiveattn+1125data.ipynb/]. 

- (CustomerFeedback.xlsx)[CustomerFeedback.xlsx/]: 

This dataset contains 100 customer feedbacks manually built initally to train a simple RNN model; the accuracy of the model did not surpass 70% on the training dataset and 43% on the testing dataset. The additive attention model is then applied to the model and performs exceptionally well even with a very limited training dataset. The results can be found (here)[Addatten_100.ipynb/].




