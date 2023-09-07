# Loan Status Prediction using Support Vector Machines

This repository contains a machine learning project that predicts loan approval status using a Support Vector Machine (SVM) model. The dataset used in this project includes information about loan applicants, such as gender, marital status, education, employment, property area, and loan approval status (approved or not approved).

## Dataset
https://www.kaggle.com/datasets/ninzaami/loan-predication

## Project Overview

The project is divided into the following sections:

1. **Data Collection and Processing**: We begin by loading the dataset, performing initial data exploration, handling missing values, and encoding categorical variables to prepare the data for modeling.

2. **Data Visualization**: Visualizations are used to gain insights into the relationships between features and loan approval status. We visualize the impact of education, marital status, and other factors on loan approval.

3. **Data Splitting**: The dataset is split into training and testing sets to evaluate the SVM model's performance. We use 90% of the data for training and 10% for testing, ensuring that the classes are stratified.

4. **Training the SVM Model**: We train a Support Vector Machine (SVM) model with a linear kernel using the training data.

5. **Model Evaluation**: The accuracy of the SVM model is evaluated on both the training and testing datasets. This helps us assess how well the model performs in predicting loan approval status.

By the end of this project, you'll have a working understanding of how to build a loan status prediction model using an SVM classifier and how to assess its accuracy. You can further explore different machine learning algorithms or feature engineering techniques to improve predictive performance.

## Getting Started

To use this project, follow these steps:

1. Clone the repository to your local machine:

2. Install the required libraries specified in the Jupyter Notebook.

3. Run the Jupyter Notebook `Loan_Status_Prediction.ipynb` to perform data exploration, model training, and evaluation.

4. Modify the code or dataset as needed for your specific use case.

## Dependencies

- numpy
- pandas
- seaborn
- sklearn

## Dataset Source

The dataset used in this project can be found [here](https://example.com/dataset).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Special thanks to the contributors and maintainers of the libraries and tools used in this project.

Feel free to contribute or provide feedback to improve this project.

