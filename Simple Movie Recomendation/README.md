
# Movie Recommendation System using Content-Based Approach
## Introduction
This code example demonstrates the creation of a content-based movie recommendation system using Python. The system suggests movies to users based on similarities in their textual attributes, such as plot summaries, genres, actors, and directors. The key principles covered in this code include data preprocessing, feature extraction, cosine similarity calculation, and movie recommendation.

## Dataset Information
The dataset used in this example comprises movie data collected from IMDB, potentially including television content. Movie information is organized using Movie IDs obtained from Kaggle projects. The dataset consists of over 5000 observations with 27 variables, providing a comprehensive foundation for building the recommendation system.

## Dependencies
Ensure you have the following Python libraries installed:

<li>pandas
<li>numpy
<li>re
<li>nltk
<li>scikit-learn

## Code Explanation
### Data Preprocessing
<li>Text Cleaning and Lowercasing: The 'Plot' column of the dataset is converted to lowercase, and non-alphabet characters are substituted with spaces to ensure consistent and uniform text data.

<li>Tokenization: Plot descriptions are tokenized into individual words using the nltk library's word_tokenize function. This process breaks down the text into manageable units for analysis.

<li>Stopword Removal: Common English stopwords are removed from tokenized plot descriptions to retain only meaningful words, improving the relevance of text data.

<li>Genre, Actors, and Director Transformation: The 'Genre,' 'Actors,' and 'Director' columns are split by commas to convert comma-separated values into lists of individual items. This enables easier manipulation and analysis.

<li>Text Cleaning and Lowercasing (Again): A custom cleaning function (clean) is applied to each item in the 'Genre,' 'Actors,' and 'Director' lists. This function converts words to lowercase and removes spaces, ensuring consistent formatting.

<li>Combining Columns: Text data from 'clean_plot,' 'Genre,' 'Actors,' and 'Director' columns is combined into a single 'clean_input' column. This column represents a cohesive input containing relevant information about each movie.

<li>Final DataFrame: The DataFrame is updated to include only the 'Title' and 'clean_input' columns, which serve as the foundation for subsequent analysis.

### Feature Extraction
<li>TF-IDF Vectorization: Textual data from the 'clean_input' column is transformed into numerical features using TF-IDF vectorization from scikit-learn. TF-IDF captures word importance in movie descriptions, generating a features matrix where each row corresponds to a movie.

<li>Cosine Similarity Calculation: The cosine_similarity function computes the cosine similarity between movie pairs based on their TF-IDF feature vectors. The resulting cosine similarity matrix represents content resemblance between movies.

## Movie Recommendation
A movie recommendation function, recommend_movies(title), is provided:

<li>Given a movie title, the function identifies the index of the movie in the DataFrame.
<li>It calculates the cosine similarity scores between the input movie and other movies.
<li>The top-ranked similar movies are extracted and presented as recommendations.

## Practical Application
This code example showcases the construction of a content-based recommendation system, where data preprocessing, feature extraction, and cosine similarity computation play pivotal roles. The system enhances user experience by suggesting movies with comparable themes, genres, and plots, contributing to improved user interactions and engagement.

This code serves as a foundation for more advanced recommendation systems and demonstrates the synergy between natural language processing, data transformation, and similarity calculations. It provides a valuable reference for anyone interested in building content-based recommendation systems for various domains.

## Usage
To use this code, follow these steps:

<li>Ensure you have the required dependencies (pandas, numpy, re, nltk, scikit-learn) installed.
<li>Load the provided dataset (e.g., "IMDB_Top250Engmovies2_OMDB_Detailed.csv").
<li>Run the code cells sequentially in your preferred Python environment.
<li>You can modify the recommend_movies function to input your desired movie title and receive personalized recommendations based on the content-based approach.

Feel free to explore and adapt this code to suit your specific use case and dataset. Happy coding!