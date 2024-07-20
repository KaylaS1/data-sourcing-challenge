# Merged and cleaned up movie data obtained from NYTimes and The Movie DB using APIs

## My Code Logic
1. Used a .env file to store my API keys for the NYTimes and the Movie DB.
1. Fetched 20 pages of movie review data from the NYTimes with "love" in the headline.
1. Cleaned up data in 2 columns - title and keywords.
1. Stored all the cleaned up titles in a list for use with the next API.
1. Fetched the movie_id from the Movie DB using the titles from the NYTimes query.
1. Used the movie_id to fetch the full movie details from the Movie DB.
2. Merged both data sets using an inner join, on column "title".
1. Removed unnecessary characters from the merged file columns, deleted duplicate rows, dropped one column and reset the index.
1. Wrote the cleaned up data to a CSV file called MergedMovies, into the same directory as this code.

## Sources of code
* Most of my code is based on code provided in Week 6 Data Sourcing Activities of Columbia University's AI bootcamp