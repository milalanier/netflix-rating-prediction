# Netflix Movie Rating Prediction

## Project Overview
This project build a machine learning regression model to predict Netflix movie ratings using basic movie attributes such as duration, release year, and popularity related features. 
The goal is to explore whether easily available metadata can explain variations in audience ratings.

A linear regression model was selected to keep the project interpretable, clean, and focused on understanding relationships between features and ratings.

## Dataset

The dataset contains information on Netflix titles, including:
* Movie title
* Release year
* Duration (in Minutes)
* Rating
* Number of Votes
* Genre
* Certificate
* Description
* Stars
* Votes

Only movies were included in the analysis. TV shows were excluded to ensure consistent duration measurements

## Data Cleaning & Feature Engineering

Key preprocessing steps included:
* Converting the duration column from strings (ex: "90 mins" to a numeric feature (duration in mins)
* Handling missing values
* Selecting numberic features suitable for regression
* Scaling features using StandardScaler

## Model
* Model Type: Linear Regression
* Train/Test Split: 80%/20%
* Target Variable: Movie Rating

  The model was trained using Scikit learn pipeline to ensure clean preprocessing and reproducibility.

  ## Evaluation Metrica

  Model performance was evaluated using:
  * R2 score
  * Mean Absolute Error (MAE)
  * Root Mean Squared Error (RMSE)
 
    An Actual vs Preducted plot was used to visually assess prediction accuracy.

  ## Key Observation

  The model tends to predict values near the mean movie rating, overestimating low-rated movies and underestimating high-rated movies.
  This behavior highlights the limitations of linear regression when modeling subjective outcomes like audience ratings.

  ## Results Summary
  * The model explains a modest portion of rating variability
  * Average prediction error is approx. 1 movie rating point
  * Results demonstrate a complete end-to-end machine learning workflow
 
  ## Next Steps
  Potential improvements include:
  * Encoding genres and certifications
  * Incorporating cast and director popularity features
  * Applying models like Ridge/Lasso
  * Using NLP technique on movie descriptions
 
  ## Tools and Technologies
  * Python
  * Pandas, NumPy
  * Scikit-Learn
  * Matplotlib, Seaborn
  * Google Collab
  
  Project Structure

  |___ netflix_rating_predictions.ipynb
  |___ README.md
  |___ data/
    |__ netflix_movies.csv

  ## How to Run
    1. Clone the repository
    2. Open the notebook in Google Colab
    3. Run cells from top to bottom
 
## Author
### Jamila Lanier
