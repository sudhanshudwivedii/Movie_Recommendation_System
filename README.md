# 🎬 Movie Recommendation System

A content-based movie recommender built with NLP. It converts movie text (plot overview, genres, keywords) into TF-IDF vectors and finds the most similar movies using cosine similarity.

📓 [View the notebook](Movie_Recommendation_System.ipynb)

## Problem Statement
With thousands of movies available, it is hard to find ones you will enjoy. This project recommends similar movies by comparing their text descriptions.

## How It Works
1. Load and clean the movie metadata
2. Combine the text features (overview, genres, keywords) into one column
3. Convert the text to vectors with TF-IDF (Term Frequency-Inverse Document Frequency)
4. Compute cosine similarity between all movies
5. Return the top 10 movies most similar to the one the user picks

## Tech Stack
Python, Pandas, NumPy, Scikit-learn

## Dataset
This project uses [The Movies Dataset](https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset) by Rounak Banik on Kaggle.

- **File used:** `movies_metadata.csv`
- **Size:** about 45,000 movies released on or before July 2017
- **Features used:** overview, genres, keywords

*This product uses the TMDB API but is not endorsed or certified by TMDB.*

## Example
**Input:** The Dark Knight

**Recommendations:**
1. [paste your first result]
2. [paste your second result]
3. [paste your third result]

## How to Run
1. Clone this repository
2. Download `movies_metadata.csv` from the Kaggle link above and place it in the project folder
3. Install the libraries: `pip install -r requirements.txt`
4. Open `Movie_Recommendation_System.ipynb` in Jupyter or Google Colab and run all cells

## Project Files
- `Movie_Recommendation_System.ipynb`: full code and explanation
- `*.pkl` files: saved TF-IDF model and similarity data

## Future Improvements
- Build a Streamlit web app for a live demo
- Try BERT / Sentence-Transformers embeddings
- Add a hybrid model with collaborative filtering
- Add evaluation metrics

## Author
[Your Name] | [GitHub](https://github.com/sudhanshudwivedii) | [LinkedIn](paste-your-linkedin-link)
