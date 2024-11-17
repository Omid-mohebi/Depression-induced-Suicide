# Depression Prediction from Narrative Texts

This project aims to predict the likelihood of depressed mood based on narrative text data. The model utilizes logistic regression to classify the data derived from two narrative columns: `NarrativeLE` and `NarrativeCME`. The dataset consists of training and test data, which are processed and tokenized to create a feature set for the model.

## Table of Contents

- Installation
- Usage
- Data Description
- Model Training
- Results
- File Structure


## Installation

To run this project, you need to have Python installed along with the following libraries:

- pandas
- numpy
- nltk
- scikit-learn

You can install the required libraries using pip:

```bash
pip install pandas numpy nltk scikit-learn
```

## Usage

1. Place your `train.csv` and `test.csv` files in the same directory as the script.
2. Run the script in a Jupyter Notebook or any Python environment.
3. The model will process the data, train on the training set, and predict the depressed mood on the test set.
4. The results will be saved in a `submission.csv` file.

## Data Description

- **train.csv**: Contains the training data with columns `NarrativeLE`, `NarrativeCME`, and `DepressedMood`.
- **test.csv**: Contains the test data with columns `NarrativeLE` and `NarrativeCME`.

## Model Training

The model is trained using the following steps:

1. **Data Loading**: Load the training and test datasets.
2. **Text Processing**: Combine the narrative columns and tokenize the text while removing stop words.
3. **Vectorization**: Create a document-term matrix for both training and test datasets.
4. **Model Training**: Split the training data into training and validation sets, and fit a logistic regression model.
5. **Prediction**: Predict the depressed mood on the test dataset.

## Results

The model achieved an accuracy of approximately 100% (overfit I know..) on the training set and 78% on the test set. The predictions are saved in a CSV file named `submission.csv`.

## File Structure

```
.
├── train.csv
├── test.csv
├── submission.csv
├── Suicide.ipynb
└── result.zip

```
