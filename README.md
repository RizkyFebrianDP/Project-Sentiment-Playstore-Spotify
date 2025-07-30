# Spotify Play Store Review Sentiment Analysis

This project performs sentiment analysis on Spotify reviews scraped from the Google Play Store. It includes two main components: a web scraper to collect the review data and a sentiment analysis model to classify the reviews as positive or negative.

## Project Structure

- `src/Scraping_Spotify_Playstore.ipynb`: Jupyter notebook for scraping Spotify reviews from the Google Play Store.
- `src/dataset/dataset_scraping.csv`: The scraped dataset of Spotify reviews.
- `src/models/Sentiment_Spotify_Play_Store.ipynb`: Jupyter notebook for performing sentiment analysis on the scraped data.
- `requirements.txt`: A list of Python dependencies required to run the project.

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/your-repository.git
   cd your-repository
   ```

2. **Install the required dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

## Usage

### 1. Scraping the Data

To scrape the latest reviews from the Google Play Store, run the `src/Scraping_Spotify_Playstore.ipynb` notebook. This will generate a new `dataset_scraping.csv` file in the `src/dataset` directory.

### 2. Sentiment Analysis

To perform sentiment analysis on the scraped data, run the `src/models/Sentiment_Spotify_Play_Store.ipynb` notebook. This notebook will:
- Load the scraped data.
- Preprocess the text data.
- Perform sentiment analysis using a lexicon-based approach.
- Train and evaluate both a Random Forest and a Logistic Regression model.

## Models

This project uses two different machine learning models for sentiment analysis:

- **Random Forest:** An ensemble learning method that operates by constructing a multitude of decision trees at training time and outputting the class that is the mode of the classes (classification) or mean prediction (regression) of the individual trees.
- **Logistic Regression:** A statistical model that in its basic form uses a logistic function to model a binary dependent variable.

## Results

The performance of the models is evaluated based on their accuracy. The results are printed at the end of the `Sentiment_Spotify_Play_Store.ipynb` notebook.
