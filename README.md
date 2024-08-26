# Content-Based Movie Recommender Using Machine Learning

This project is a Content-Based Movie Recommender System developed using Python, Machine Learning, Flask, and SQL. It suggests movies to users based on the content of previously enjoyed films by leveraging a content-based filtering approach.

# Project Overview
The project consists of various stages, each with a specific focus on creating, developing, and deploying the recommender system:

## Stage 1: Data Collection (Web Scraping)
Objective: Collect movie data from the IMDb website.</br>
Method: Python's Selenium library was used to scrape movie metadata, including titles, genres, directors, plot summaries, and user votes.</br>
Outcome: The collected data was saved into a CSV file, which serves as the primary data source for the recommendation engine.</br>

## Stage 2: Data Processing and Cleansing
Objective: Prepare the scraped data for building the recommender system.</br>
Method: The data was cleaned by removing null values, duplicates, and standardizing user votes format. Additionally, genres were label-encoded to make the data suitable for machine learning models.</br>
Outcome: The cleansed and processed data was loaded into a MySQL database for easy retrieval and querying.</br>

## Stage 3: Machine Learning Model Development
Objective: Build the content-based movie recommender using the TF-IDF (Term Frequency-Inverse Document Frequency) algorithm.</br>
Method: A TF-IDF matrix was computed from movie plot summaries to understand the textual relevance between different movies. The cosine similarity measure was used to compare movies based on this matrix and generate recommendations.</br>
Outcome: A Python script was developed to process user input, compute similarity scores, and recommend movies that match user preferences.</br>

## Stage 4: Building a Flask Web Application
Objective: Develop a user-friendly web application to interact with the recommendation engine.</br>
Method: A Flask-based web app was created that allows users to input their movie preferences. The app retrieves data from the MySQL database and generates recommendations based on the TF-IDF model.</br>
Outcome: A fully functional web application deployed on Google Cloud Platform (GCP), where users can receive personalized movie suggestions.</br>

## Stage 5: Deployment and Testing
Objective: Deploy the application for public use and ensure its performance.</br>
Method: The Flask app was deployed using GCP Compute Engine, and various test cases were run to ensure the recommender system works effectively for diverse inputs.</br>
Outcome: The project was successfully deployed, and the system is capable of generating accurate movie recommendations based on content similarity.</br>

# Technologies Used
Programming Languages: Python, SQL</br>
Web Scraping: Selenium</br>
Machine Learning: TF-IDF, Cosine Similarity</br>
Web Framework: Flask</br>
Database: MySQL</br>
Cloud Platform: Google Cloud Platform (GCP)</br>

# Future Scope
Incorporating User Ratings: Introduce a hybrid recommendation system by integrating collaborative filtering with content-based filtering to improve recommendation quality.</br>
Expansion of Data Sources: Increase the dataset by scraping more comprehensive movie information from various platforms beyond IMDb.</br>
Performance Optimization: Optimize the model's performance for real-time movie recommendations.</br>

