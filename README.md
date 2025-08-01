README.md
markdown
Copy code
# Movie Review Sentiment Classifier using NLTK and Logistic Regression

This project is a basic NLP pipeline that classifies movie reviews as **positive** or **negative** using the **NLTK Movie Reviews dataset** and **Logistic Regression**.

## 🔍 What This Code Does

1. **Loads the Movie Review Dataset**  
   - Uses `nltk.corpus.movie_reviews` to get 2000 labeled reviews (1000 positive, 1000 negative).

2. **Creates a DataFrame**  
   - Organizes the review text and corresponding sentiment labels into a Pandas DataFrame.

3. **Encodes the Data**  
   - Applies `TfidfVectorizer` to convert raw text reviews into numerical feature vectors.
   - Uses `LabelEncoder` to convert sentiment labels into 0 (negative) and 1 (positive).

4. **Trains a Logistic Regression Model**  
   - Splits the data into training and testing sets.
   - Fits a `LogisticRegression` model using the training data.

5. **Evaluates the Model**  
   - Prints accuracy, classification report, and confusion matrix for the test set.

6. **Allows Custom Review Testing**  
   - Accepts user input from the terminal.
   - Predicts the sentiment of the custom input review.
   - Displays the predicted sentiment along with the model’s test accuracy.
