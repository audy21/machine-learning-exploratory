# Book Recommendation System using K-Nearest Neighbors (KNN)

This project implements a book recommendation system using the K-Nearest Neighbors (KNN) algorithm. The system recommends books based on user ratings, finding similar books using cosine similarity as the distance metric.

## Project Structure

The notebook contains the following main sections:

### 1. Data Loading and Preparation
- Imports necessary libraries: **NumPy**, **Pandas**, **SciPy**, **scikit-learn**.
- Loads book and rating data from CSV files.
- Cleans data by:
    - Removing null values.
    - Filtering out users with fewer than 200 ratings.
    - Filtering out books with fewer than 100 ratings.

### 2. Data Transformation
- Creates a pivot table with:
    - Books as rows.
    - Users as columns.
    - Ratings as values.
- Joins book titles to the rating data for better readability.

### 3. Model Building
- Initializes a KNN model using the cosine similarity metric.
- Fits the model to the prepared data.

### 4. Recommendation Function
- Implements the `get_recommends()` function:
    - Takes a book title as input.
    - Finds the 5 most similar books using the KNN model.
    - Returns recommendations with similarity scores.

### 5. Testing
- Includes a test case to verify that the recommendation function works correctly.

## Key Features
- Uses a collaborative filtering approach based on user ratings.
- Implements cosine similarity to find books with similar rating patterns.
- Handles data sparsity by filtering inactive users and unpopular books.
- Provides a clean interface through the `get_recommends()` function.

## Usage

To get book recommendations, use the following code:

```python
recommendations = get_recommends("The Queen of the Damned (Vampire Chronicles (Paperback))")
print(recommendations)
```

## Dependencies
- Python 3.x
- NumPy
- Pandas
- scikit-learn
- SciPy

## Data Sources
The project uses two CSV files:
- **BX-Books.csv**: Contains book information (ISBN, title, author).
- **BX-Book-Ratings.csv**: Contains user ratings for books.
