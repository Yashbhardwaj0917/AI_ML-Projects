# Fake News Article Detection using Natural Language Processing

This repository contains a machine learning model for classifying news articles as either "Real" or "Fake" based on their content. The model is built using Natural Language Processing (NLP) techniques and Logistic Regression.

## Dataset

https://www.kaggle.com/c/fake-news/data?select=train.csv

The dataset used in this project is loaded from a CSV file and includes information such as the author, title, and content of each news article. The goal is to create a model that can effectively distinguish between genuine news articles and fake or misleading ones.

## Data Preprocessing

1. **Combining Author and Title**: The "author" and "title" columns are concatenated into a single "content" column to capture more information for classification.

2. **Text Preprocessing**: Text data is cleaned by converting it to lowercase, removing non-alphabetical characters, and applying word stemming using the Porter Stemmer. Common English stopwords are also removed to focus on meaningful words.

## Feature Engineering

Text data is converted into numerical features using the TF-IDF (Term Frequency-Inverse Document Frequency) vectorization technique. This process transforms the text into numerical features while considering the importance of words in the corpus.

## Model Building

A Logistic Regression classifier is utilized to train the model. Logistic Regression is a popular choice for text classification tasks due to its simplicity and effectiveness.

## Model Evaluation

The model's performance is assessed by calculating accuracy scores on both the training and testing datasets. Additionally, a sample from the test data is selected, and predictions are made to demonstrate how the model classifies news articles.

## Getting Started

To use this project, follow these steps:

1. Clone the repository to your local machine:

2. Install the required dependencies:

3. Run the Jupyter Notebook `fake_news_detection.ipynb` to build and evaluate the model.

4. Modify the code or dataset as needed for your specific use case.

## Dependencies

- numpy
- pandas
- nltk
- sklearn

## Dataset Source

The dataset used in this project can be found [here](https://example.com/dataset).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Special thanks to the contributors and maintainers of the libraries and tools used in this project.

Feel free to contribute or provide feedback to improve this project.


