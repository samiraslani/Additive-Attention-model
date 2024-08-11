# Machine Translation 
## Bi-directional LSTM Attention Model 
 
The goal of this project is to create an attention model that is able to recognize human-readable dates and translate them to machine-readable dates. This project is part of the labs offered in the course [Sequence Learning](https://www.coursera.org/learn/nlp-sequence-models ) by DeepLearning.ai. More explanation on the structure of the model can be found [here](AttentionModelCoursera.ipynb/)

The attention model built is based on the paper by [Bahdanau et al., 2014](https://doi.org/10.48550/arXiv.1409.0473). 

The file [nmt_utils.py](nmt_utils.py/) creates the arbitary human-readable dates to train the model with. A pdf file on how the attention mechanism in this project works is also added: [Notes](Notes.pdf)

The trained weights can be found on the file [model_weights.weights.h5](model_weights.weights.h5/). 

