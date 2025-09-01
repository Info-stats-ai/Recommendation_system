# Netflix Movie Recommendation Project

This project aims to build a movie recommendation system using the Netflix Prize dataset. The goal is to predict how a user will rate a movie they have not yet seen, based on their past ratings and the ratings of other users.

## Project Overview

The project involves the following steps:

1.  **Data Loading and Preparation**: Load the Netflix Prize dataset, which consists of multiple files containing movie ratings. The data is combined and preprocessed for analysis.
2.  **Exploratory Data Analysis (EDA)**: Analyze the distribution of ratings, the number of ratings per user and per movie, and the temporal trends in ratings.
3.  **Data Splitting**: Split the data into training and testing sets based on time to simulate a real-world scenario where recommendations are made for future ratings.
4.  **Sparsity Analysis**: Examine the sparsity of the user-movie rating matrix, which is a common characteristic of recommendation system datasets.
5.  **Baseline Models**: Implement and evaluate baseline recommendation models such as the global average, user average, and movie average ratings.
6.  **Collaborative Filtering Models**: Explore collaborative filtering techniques, including user-based and item-based methods (e.g., using KNN algorithms from the Surprise library).
7.  **Matrix Factorization Models**: Implement and evaluate matrix factorization models like Singular Value Decomposition (SVD) and SVD++ using the Surprise library.
8.  **Hybrid Models**: Combine features from different models (e.g., baseline predictions, KNN predictions, SVD predictions) to train a regression model (XGBoost) for improved prediction accuracy.
9.  **Model Evaluation**: Evaluate the performance of different models using metrics such as Root Mean Squared Error (RMSE) and Mean Absolute Percentage Error (MAPE).
10. **Hyperparameter Tuning**: Optimize the performance of the chosen models by tuning their hyperparameters using techniques like GridSearchCV and k-fold cross-validation with early stopping.

## Dataset

The dataset used in this project is the Netflix Prize dataset, which can be obtained from [link to dataset if available, otherwise mention it's a public dataset]. It contains anonymized rating data from Netflix users.

## Requirements

To run this project, you need to install the following libraries:

-   pandas
-   numpy
-   matplotlib
-   seaborn
-   scipy
-   scikit-learn
-   surprise
-   xgboost

You can install these libraries using pip as described in the `requirements.txt` file.

## Usage

1.  Clone the repository: `git clone <repository_url>`
2.  Navigate to the project directory: `cd <project_directory>`
3.  Install the required libraries: `pip install -r requirements.txt`
4.  Run the Jupyter Notebook or Python scripts to execute the project steps.

## File Structure

-   `README.md`: This file.
-   `requirements.txt`: Lists the required Python libraries.
-   `notebook.ipynb`: The Jupyter Notebook containing the project code and analysis.
-   `combined_data_*.txt`: The raw data files (assuming they are included or downloaded separately).
-   `movie_titles.csv`: Contains movie titles corresponding to movie IDs.
-   `data.csv`: The combined and preprocessed rating data.
-   `train.csv`: The training dataset.
-   `test.csv`: The testing dataset.
-   `sample_train_sparse_matrix.npz`: Sampled sparse matrix for training (saved in NPZ format).
-   `sample_test_sparse_matrix.npz`: Sampled sparse matrix for testing (saved in NPZ format).
-   `reg_train.csv`: Training data with features for regression models.
-   `reg_test.csv`: Testing data with features for regression models.

## Results

The notebook includes the results of the data analysis, model training, and evaluation. The performance of different models is compared based on RMSE and MAPE.
