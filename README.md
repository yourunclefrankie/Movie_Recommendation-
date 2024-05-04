---

# Collaborative Filtering for Game Recommendation with PySpark

This repository contains code for collaborative filtering using PySpark's ALS algorithm to recommend games based on user preferences.

## Overview

Collaborative filtering is a popular technique in recommendation systems. This project focuses on building a recommendation system for games using PySpark's ALS algorithm.

## Requirements

- Python 3.x
- PySpark
- Pandas
- Matplotlib
- MLflow

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/yourunclefrankie/recommendation-system.
   cd recommendation-system
   ```
2. Install the required dependencies:
   ```
   pip install pyspark pandas matplotlib mlflow
   ```
## Usage

1. Ensure you have the dataset `steam_200k__1_.csv` available.
2. Update the file path in the code to point to your dataset.
3. Run the script `recommendation_system.py`:
   ```
   python recommendation_system.py
   ```

## Code Structure

- `recommendation_system.py`: Main script containing the code for collaborative filtering and model evaluation.
- `README.md`: Instructions and information about the project.

## Data Preprocessing

- Reads the dataset into a Spark DataFrame.
- Handles missing values by dropping them.
- Removes duplicate rows.
- Assigns unique IDs to game titles for efficient processing.

## Model Training and Evaluation

- Splits the data into training and test sets.
- Trains an ALS model using PySpark.
- Evaluates the model's performance using RMSE.
- Performs hyperparameter tuning using TrainValidationSplit.
- Selects the best model based on evaluation metrics.

## Visualization

- Displays the distribution of purchases and plays.
- Visualizes the total playtime for each game.
- Plots a box plot of ratings to identify outliers.

## Acknowledgments

- PySpark Documentation: https://spark.apache.org/docs/latest/api/python/index.html
- MLflow Documentation: https://www.mlflow.org/docs/latest/index.html

---


