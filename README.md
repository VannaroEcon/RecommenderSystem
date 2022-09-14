# RecommenderSystem

This repository includes the data and notebook for the movie recommender system. We aim to build a system to recommend similar movies to the audience given the movie that he/she previously watched or liked. We go a step further by making this recommender system work with Japanese text. 

## Data

Data (IMDB movies) is obtained from data.world. Originally, the data is in English, but then translated into Japanese to match this study objective.

- First, the data was uploaded to Google Drive and then converted into Google Sheet. 
- Then, we tranlated those data to Japanese using GOOGLETRANSLATE function.
- Finally, we cleaned up the data and kept only necessary columns for our analysis.

## Method

This recommender is a content-based recommender using Natural Language Processing (NLP) which follows the below steps:
1. Remove stopwords and punctuation to extract keywords from synopsis.
2. Generate word representation for each movie based on director name, actor name, genre, and synopsis.
3. Generate vector representation.
4. Calculate cosine similirarity index for each movie.
5. Recommend the most similar movies given the title of movie that the audience liked.

## Result

We succesfully extract keywords from Japanese text by applying customized RAKE fuction.
The recommended movies are mostly identical for both Japanese and English recommenders. This result implies that our Japanese recommender works well, and we are able to recommend the right movies that audience might like based on Japanese text/synopsis.
