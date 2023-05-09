# U.S.-Patent-Phrase-to-Phrase-Matching-NLP

## Introduction
This project aims to match phrases in US patents using natural language processing (NLP) techniques. The dataset contains pairs of phrases, an anchor phrase and a target phrase, along with a context phrase, and a score indicating the level of similarity between the anchor and target phrases. The task is to predict this similarity score for a test set of phrase pairs.
## Approach
Data Preparation: The data is prepared by loading it from Kaggle or local storage. The dataset is then converted into a suitable format for further processing.

Tokenization: The input text is tokenized using the DeBERTa V3 tokenizer from the Transformers library.

Dataset Splitting: The dataset is split into training and validation sets using a 75% / 25% split ratio. A separate test set is also used for evaluation.

Training: The model is trained using the Trainer class from the Transformers library. The learning rate, batch size, and number of epochs are set as hyperparameters.

Evaluation: The model is evaluated using the Pearson correlation coefficient as a metric. The evaluation is performed on the validation set and test set.

Prediction: The model is used to make predictions on the test set

## Dependencies

This project uses the following dependencies:

- Python 3.7 or higher
- PyTorch
- Transformers
- Pandas
- Scikit-learn
- Kaggle
