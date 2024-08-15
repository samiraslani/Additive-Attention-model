# Machine Translation 
## Bi-directional LSTM Attention Model 
 
The goal of this project is to first understand the mechanisms applied to construct an attention model by creating a machine translation model, which is able to recognize human-readable dates and translate them to machine-readable dates. This project is part of the labs offered in the course [Sequence Learning](https://www.coursera.org/learn/nlp-sequence-models ) by DeepLearning.ai. More explanation on the structure of the model can be found [here](AttentionModelCoursera.ipynb/).

We will then apply the attention procedure to train a sentiment analysis model based on the dataset Canva_reviews.xlsx. This dataset is part of the project "Build Multi Class Text Classification Models with RNN and LSTM" from [ProjectPro](https://www.projectpro.io/). We will use two embeddings for words one with one-hot vectors and another with GloVe embeddings. The accuracy of the model reached 98% on the training set(1125 sample feedbacks) and 91% on the testing set (375 sample feedbacks). 



The attention model built is based on the paper by [Bahdanau et al., 2014](https://doi.org/10.48550/arXiv.1409.0473). 

The file [nmt_utils.py](nmt_utils.py/) creates the arbitary human-readable dates to train the model with. A pdf file on how the attention mechanism in this project works is also added: [Notes](Notes.pdf)

The trained weights for both projects are saved as: [model_weights.weights.h5](model_weights.weights.h5/) (for the machine translation task), [attention_hotV1125.weights.h5](attention_hotV1125.weights.h5/) (for the sentiment analysis with one-hot vector encoding) and [attention_GloV1125.weights.h5](attention_GloV1125.weights.h5/) (for sentiment analysis with GloVe embeddings). 

