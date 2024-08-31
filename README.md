# Additive Attention Model

## Project Overview

This project focuses on implementing an attention model for machine translation with a specific application: converting human-readable dates into machine-readable formats. The project is part of the Sequence Learning course by DeepLearning.ai and leverages concepts from the paper by Bahdanau et al. (2014) on attention mechanisms.

## Components

### Attention Model

The primary component is a machine translation model utilizing an attention mechanism. For detailed information on the model's structure and functionality, refer to [this resource](link-to-resource).

### Utilities

- **`nmt_utils.py`**: Contains functions to generate arbitrary human-readable dates for training the model.

### Additive Attention Mechanism

For a comprehensive explanation of how the additive attention mechanism works, see [Additive Attention Notes](link-to-notes).

### Sentiment Analysis

We also apply the attention mechanism to sentiment analysis using two datasets:

1. **Canva_reviews.xlsx**
   - **Description**: Contains 1,500 customer feedback entries for the Canva app. This dataset is sourced from the "Build Multi-Class Text Classification Models with RNN and LSTM" project by ProjectPro.
   - **Embeddings Used**: One-hot vectors and GloVe embeddings.
   - **Results**: Check the results in [Additiveattn+1125data.ipynb](link-to-notebook).

2. **CustomerFeedback.xlsx**
   - **Description**: Contains 100 manually created customer feedback entries. Initially used to train a basic RNN model, which achieved an accuracy of 70% on the training set and 43% on the test set.
   - **Results**: Applying the additive attention model showed significant improvement. Detailed results are available in [Addatten_100.ipynb](link-to-notebook).

## Getting Started

To get started with this project, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/username/repository-name.git

2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt

3. **Run Notebooks**:
   Open the Jupyter Notebooks (*.ipynb files) to explore model implementations and results.
## Contributing

If you’d like to contribute to this project, please fork the repository and submit a pull request with your proposed changes.

## License

This project is licensed under the MIT License. See the [LICENSE](link-to-license) file for details.

## Acknowledgments

- DeepLearning.ai for the Sequence Learning course.
- Bahdanau et al. (2014) for their foundational work on attention mechanisms.
- ProjectPro for providing the sentiment analysis dataset.






























# Machine Translation 
## Bi-directional LSTM Attention Model 
 
The goal of this project is to first understand the mechanisms applied to construct an attention model by creating a machine translation model, which is able to recognize human-readable dates and translate them to machine-readable dates. This project is part of the labs offered in the course [Sequence Learning](https://www.coursera.org/learn/nlp-sequence-models ) by DeepLearning.ai. More explanation on the structure of the model can be found [here](Machine_translation.ipynb/). The attention model built is based on the paper by [Bahdanau et al., 2014](https://doi.org/10.48550/arXiv.1409.0473). 

Furthermore, the file [nmt_utils.py](nmt_utils.py/) creates the arbitary human-readable dates to train the model with. Some notes on how the additive attention mechanism works is also added: [Notes](Notes.pdf)

We will then apply the attention procedure to train a sentiment analysis model based on two datasets: 
- [Canva_reviews.xlsx](Canva_reviews.xlsx/): 

This dataset contains 1500 customer feedbacks for the app Canva and is part of the project "Build Multi Class Text Classification Models with RNN and LSTM" from [ProjectPro](https://www.projectpro.io/). We will use two embeddings for words one with one-hot vectors and another with GloVe embeddings. To check the resutls please check the file [Additiveattn+1125data.ipynb](Additiveattn+1125data.ipynb/). 

- [CustomerFeedback.xlsx](CustomerFeedback.xlsx/)

This dataset contains 100 customer feedbacks manually built initally to train a simple RNN model; the accuracy of the model did not surpass 70% on the training dataset and 43% on the testing dataset. The additive attention model is then applied to the model and performs exceptionally well even with a very limited training dataset. The results can be found [Addatten_100.ipynb](Addatten_100.ipynb/).




