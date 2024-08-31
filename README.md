# Additive Attention Model

## Project Overview

This project focuses on implementing an additive attention model for machine translation with a specific application: converting human-readable dates into machine-readable formats. The project is part of the [Sequence Learning](https://www.coursera.org/learn/nlp-sequence-models) course by [DeepLearning.ai](deeplearning.ai) and leverages concepts from the paper by [Bahdanau et al. (2014)](https://doi.org/10.48550/arXiv.1409.0473).

In addition, the additive attention model is applied to the task of sentiment analysis using two different datasets to examine the performance of the model. 

## Components

### Machine Translation

The primary component is a machine translation model utilizing an attention mechanism. For detailed information on the model's structure and functionality, refer to [Machine_translation.ipynb](Machine_translation.ipynb/).

### Utilities

- **`nmt_utils.py`**: Contains functions to generate arbitrary human-readable dates for training the model.
- **`Notes.pdf`**: Contains detailed complementary notes on the attention model. 


### Sentiment Analysis

We apply the attention mechanism to sentiment analysis using two datasets:

1. **Canva_reviews.xlsx**
   - **Description**: Contains 1,500 customer feedback entries for the Canva app. This dataset is sourced from the "Build Multi-Class Text Classification Models with RNN and LSTM" project by [ProjectPro](https://www.projectpro.io/)
   - **Embeddings Used**: One-hot vectors and GloVe embeddings.
   - **Results**: Check the results in [Additiveattn+1125data.ipynb](Additiveattn+1125data.ipynb/).

2. **CustomerFeedback.xlsx**
   - **Description**: Contains 100 manually created customer feedback entries. Initially used to train a basic RNN model, which did not surpass an accuracy of 90% on the training set and 43% on the testing set.
   - **Embeddings Used**: One-hot vectors and GloVe embeddings.
   - **Results**: Applying the additive attention model showed significant improvement. Detailed results are available in [Addatten_100.ipynb](Addatten_100.ipynb/).

## Getting Started

To get started with this project, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/samiraslani/Additive-Attention-model.git

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
