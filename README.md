
# Movie-Recommendation-System

A content-based Movie Recommendation System that suggests similar movies to the user based on their selection. This project uses Natural Language Processing (NLP) and machine learning techniques to analyze and recommend movies effectively.


## 🌟 Features

- Dynamic Recommendations: Suggests movies based on content similarity.
- Content Parsing: Extracts key elements like genres, keywords, cast, crew, and overview for analysis.
- Efficient Search: Provides top recommendations quickly using cosine similarity.
- Preprocessed Data: Includes pre-processed movie data for efficient use.



## 🛠️ Technologies Used

- Programming Language: Python
- Libraries:
    - Data Processing: pandas, numpy
    - NLP: nltk, ast
    - Machine Learning: scikit-learn
    - Deployment: streamlit, pickle

## 📂 Project Structure

File/Folder	Description
app.py	Flask application for the web interface.
movie_dict.pkl	Preprocessed movie data stored in pickle format.
movies.pkl	Movie metadata for recommendations.
requirements.txt	Lists all dependencies for the project.
setup.sh	Shell script for setting up the environment.
Procfile	Heroku deployment configuration.
README.md	Project documentation.
Dataset_kaggle_link	Link to the Kaggle dataset used.

## 📚 Data Overview

- Dataset Source: Kaggle's TMDB 5000 Movie Dataset

- Columns Used:
    - movie_id: Unique ID for each movie.
    - title: Title of the movie.
    - overview: Brief description of the movie.
    - genres, keywords, cast, crew: Metadata for recommendation.
## 🚀 Working

1. Data Preprocessing:
- Extract and process genres, keywords, cast, and crew columns.
- Convert metadata into lists and remove spaces for uniformity.
- Create a tags column by concatenating key metadata.
- Apply stemming to normalize words.

2. Vectorization:
- Use CountVectorizer to generate feature vectors based on top 5000 words.

3. Similarity Calculation:
- Compute pairwise cosine similarity between movie vectors.

4. Recommendations:
- Retrieve the top 5 most similar movies for a given input.
## 🖥️ Running the Project
Prerequisites

- Python 3.x installed.
- Required libraries installed via requirements.txt.

Steps:

1. Clone the repository:

```bash 
    git clone https://github.com/tejas6376/Movie-Recommendation-System
    cd Movie-Recommendation-System
```   

2. Install dependencies:

```bash 
    pip install -r requirements.txt
```   

3. Run the Streamlit app:

```bash 
    python app.py
```   





## 📈 Example
Input: Interstellar 

Output: Recommended movies based on content similarity:

- The Martian
- Gravity
- Inception
- Contact
- Ad Astra
## 🔗 Dataset
The dataset used for this project is available at Kaggle.
https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata

Or Download the datasets from the Data folder in the repository
## 🤝 Contributing
Contributions are welcome! Fork the repository and submit a pull request for any improvements.
## 📧 Contact
For any queries or suggestions, feel free to reach out:
- [Tejas Mahajan] 
- [tejasmahajan101@gmail.com] 
- [https://linkedin.com/in/tejas-mahajan-185270285/]
- [https://github.com/tejas6376]
