# 🎬 Movie Recommendation System

A content-based movie recommender built with NLP. It converts movie text (plot overview, genres, tagline) into TF-IDF vectors and finds the most similar movies using cosine similarity.

📓 [View the notebook](Movie_Recommendation_System.ipynb)

## Problem Statement
With thousands of movies available, it is hard to find ones you will enjoy. This project recommends similar movies by comparing their text descriptions.

## How It Works
1. Load `movies_metadata.csv` (45,466 rows) and remove duplicates
2. Combine overview, genres, and tagline into one text column
3. Clean the text with NLTK: lowercase, remove punctuation and stopwords, lemmatize
4. Convert the text to vectors with TF-IDF (Term Frequency-Inverse Document Frequency), using unigrams and bigrams and up to 50,000 features
5. Compute cosine similarity and return the top N movies most similar to the one the user picks

## Tech Stack
Python, Pandas, NumPy, NLTK, Scikit-learn

## Dataset
This project uses [The Movies Dataset](https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset) by Rounak Banik on Kaggle.

- **File used:** `movies_metadata.csv`
- **Size:** 45,447 movies after cleaning (released on or before July 2017)
- **Features used:** overview, genres, tagline

*This product uses the TMDB API but is not endorsed or certified by TMDB.*

## Example
**Input:** Avatar

**Top 5 recommendations:**
1. Avatar 2
2. The Inhabited Island
3. Thor: Ragnarok
4. Moontrap: Target Earth
5. The Three Musketeers

## How to Run
1. Clone this repository
2. Download `movies_metadata.csv` from the Kaggle link above and place it in the project folder
3. Install the libraries: `pip install -r requirements.txt`
4. Open `Movie_Recommendation_System.ipynb` in Jupyter or Google Colab and run all cells

## Project Files
- `Movie_Recommendation_System.ipynb`: full code and explanation
- `tfidf.pkl`, `tfidf_matrix.pkl`, `indices.pkl`: saved TF-IDF model, matrix, and title index
- `requirements.txt`: required libraries

## Future Improvements
- Add keywords, cast, and director to the text features for better matches
- Build a Streamlit web app for a live demo
- Try BERT / Sentence-Transformers embeddings
- Add a hybrid model with collaborative filtering
- Add evaluation metrics

## Author
Sudhanshu Dwivedi | [GitHub](https://github.com/sudhanshudwivedii) | [LinkedIn](https://www.linkedin.com/in/sudhanshu-dwivedi-88727b322/)
