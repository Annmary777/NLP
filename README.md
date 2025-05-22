# IMDB Movie Reviews Sentiment Analysis - Preprocessing & Feature Extraction

This project demonstrates preprocessing and feature extraction techniques applied to the IMDB movie reviews dataset for sentiment analysis. The dataset contains movie reviews labeled as positive or negative, and this code prepares the text data for use in machine learning models.

## Project Overview

- Load the IMDB movie reviews dataset.
- Map sentiment labels to binary values (`positive` → 1, `negative` → 0).
- Shuffle and split the dataset into training and testing sets.
- Clean the text by:
  - Lowercasing
  - Removing HTML tags
  - Removing stopwords and punctuation
  - Adding spaces around punctuation to aid tokenization
- Extract features using:
  - Bag of Words (unigrams)
  - Bag of Bigrams (2-grams)
  - One-Hot Encoding with `CountVectorizer` (binary presence of tokens)
- Generate bigrams manually using NLTK for deeper analysis.

## Dataset

- IMDB Dataset CSV file containing 50,000 movie reviews.
- Each review is labeled as `positive` or `negative`.

## Dependencies

- Python 3.7+
- pandas
- scikit-learn
- nltk
- beautifulsoup4
- tqdm

## How to Run

1. Clone the repository or download the notebook/script.
2. Ensure you have the dataset CSV file (`IMDB Dataset.csv`) in the project directory or update the path accordingly.
3. Install dependencies (see `requirements.txt`).
4. Run the script or notebook cells sequentially to preprocess data and extract features.

## Key Functions and Modules

- **Text Cleaning:** Uses `BeautifulSoup` to strip HTML tags, NLTK to remove stopwords, and custom punctuation handling.
- **Bigram Generation:** Uses NLTK’s `bigrams` function to create bigram sequences.
- **Vectorization:** Uses `CountVectorizer` from scikit-learn for Bag of Words, bigrams, and one-hot encoding.

## Example Output

- Total Vocabulary Size after cleaning: ~110,000 unique tokens.
- Feature matrices showing token counts and presence indicators.

## Future Work

- Train machine learning models (e.g., Logistic Regression, Naive Bayes, or deep learning models) on the extracted features.
- Perform hyperparameter tuning and cross-validation.
- Explore advanced embeddings like Word2Vec, GloVe, or BERT for improved sentiment classification.

## Contact

For questions or suggestions, please open an issue or contact [Your Name] at [your-email@example.com].

---

