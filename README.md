# Movie-Recommendation-ML-Project
This project is a content-based movie recommendation system that suggests movies similar to a user's input. By analyzing the similarity of movie descriptions, this system recommends 10 movies related to the one specified by the user.

# Project Overview
The recommendation system uses a dataset of movies, leveraging natural language processing techniques to compute similarity between movies based on their descriptions or other text-based attributes. The system uses the cosine similarity measure to find movies most similar to the user's chosen title.

# Data Set Link : 
https://drive.google.com/file/d/1cCkwiVv4mgfl20ntgY3n4yApcWqqZQe6/view?pli=1

# Technologies Used:
 - **Python**: Primary programming language
 - **NumPy**: For numerical operations
 - **Pandas**: For data handling and manipulation
 - **difflib**: For approximate string matching to handle misspelled movie titles
 - **scikit-learn**:
    - **TfidfVectorizer** for converting text data into a numerical format
    - **cosine_similarity** for calculating similarity between movies

# How It Works
 - **User Input**: The user inputs the name of a movie.
 - **Data Lookup**: The system checks the dataset for a close match to the input movie name using difflib.
 - **Feature Extraction**: TfidfVectorizer transforms the movie descriptions into numerical vectors.
 - **Similarity Calculation**: cosine_similarity measures the similarity between the input movie and all other movies in the dataset.
 - **Recommendation**: The top 10 most similar movies are returned as recommendations.
