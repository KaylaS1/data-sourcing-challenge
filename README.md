# Merged and cleaned up movie data obtained from NYTimes and The Movie DB using APIs

## Logic
1. I used a .env file to store my API keys for the NYTimes and the Movie DB.
1. I fetched 20 pages of movie review data from the NYTimes with "love" in the headline.
1. I cleaned up data in 2 columns - title and keywords.
1. I stored all the cleaned up titles in a list for use with the next API.
1. I fetched the movie_id from the Movie DB using the titles from the NYTimes query.
1. I used the movie_id to fetch the full movie details from the Movie DB.
2. I merged both data sets using an inner join, on column "title".
1. I removed unnecessary characters from the merged file columns, deleted duplicate rows, dropped one column and rest the index.
1. I wrote the cleaned up data to a CSV file called MergedMovies.

## Sources of code
* Most of my code is based on code provided in Week 6 Data Sourcing Activities