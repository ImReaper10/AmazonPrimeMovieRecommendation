# AmazonPrimeMovieRecommendation
This project analyzes the Amazon Prime Titles dataset and implements an exploratory data analysis (EDA) and a movie recommendation system using cosine similarity. The code covers data cleaning, visualization, and building a content-based recommendation system based on the cast, director, and other features.

Key Features:
**Data Cleaning:**

Loaded the dataset and inspected its structure using head() and shape().
Identified and removed missing values using dropna().
Filled in missing values for columns like director, cast, and country with "Unknown".
Dropped the date_added column as it was irrelevant.
Filled missing rating values with the mode (most frequent value).
Checked for and handled duplicate records.
**Exploratory Data Analysis (EDA):**

Visualized the distribution of content types (Movies vs TV Shows) using a pie chart.
Counted the top 10 most frequent directors in the dataset.
Created a bar plot to display the distribution of different ratings.
Analyzed content duration to find the most frequent durations.
**Movie Recommendation System:**

Used TF-IDF Vectorization to transform textual features like cast, director, listed_in (genres), and description into feature vectors.
Computed cosine similarity between movies based on these features.
Built a recommendation system that suggests similar movies based on an input movie title.
The system returns a specified number of movie recommendations based on content similarity.
**Libraries Used:**
Pandas: For data manipulation and analysis.
Seaborn: For creating statistical visualizations.
Matplotlib: For plotting graphs.
scikit-learn: For TF-IDF vectorization and cosine similarity computation.
**How to Use:**
Load the dataset (amazon_prime_titles.csv) into the project.
Clean the data by filling in missing values and dropping irrelevant columns.
Visualize insights using the provided plots and graphs.
Run the movie recommendation system by calling the recommend_movies function and inputting a movie title.
