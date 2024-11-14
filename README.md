# Amazon Fine Food Reviews Analysis

This project analyzes the Amazon Fine Food Reviews dataset to identify key variables and build predictive models. The primary objective is to understand the factors that influence review ratings and helpfulness.

## Dataset

The dataset contains reviews of fine foods from Amazon (https://www.kaggle.com/datasets/snap/amazon-fine-food-reviews?select=Reviews.csv). It includes the following columns:
- `Id`: Unique identifier for each review.
- `ProductId`: Unique identifier for each product.
- `UserId`: Unique identifier for each user.
- `ProfileName`: Name of the user.
- `HelpfulnessNumerator`: Number of users who found the review helpful.
- `HelpfulnessDenominator`: Number of users who voted on the helpfulness of the review.
- `Score`: Rating given by the user (1 to 5).
- `Time`: Timestamp of the review.
- `Summary`: Summary of the review.
- `Text`: Full text of the review.

## Project Steps

1. **Data Cleaning**: Handled missing values in `ProfileName` and `Summary`.
2. **Exploratory Data Analysis (EDA)**: Analyzed the distribution of ratings, top reviewers, review length, and helpfulness votes.
3. **Feature Engineering**: Created features like `Sentiment`, `HelpfulnessRatio`, interaction features, and text features.
4. **Model Building**: Built and evaluated a linear regression model with various features.
5. **Model Performance**: Achieved an MSE of approximately 1.35 with combined features and confirmed with cross-validation.

## Key Findings

- **Ratings Distribution**: The majority of reviews have a 5-star rating.
- **Top Reviewers**: Identified the most active reviewers.
- **Review Length**: Longer reviews tend to provide more detailed feedback.
- **Helpfulness Votes**: Positive linear relationship between the number of helpful votes and total votes.
- **Sentiment Analysis**: Sentiment scores are positively correlated with review ratings.

## Model Performance

- **Initial Model**: MSE of 1.41 using basic features.
- **Interaction Features**: Improved MSE to 1.38.
- **Text Features**: Improved MSE to 1.38.
- **Combined Features**: Further improved MSE to 1.35.
- **Cross-Validation**: Confirmed MSE of approximately 1.34 ± 0.02.

## How to Run

1. Clone the repository:
   ```bash
   git clone
