# Movie Recommendation System 
## Problem Statement
This project recommends movies similar to a given title using content-based filtering.  
It analyzes movie metadata (tags, genres, overview) and finds the closest matches.
## Dataset
- Source: TMDb-based dataset (GitHub)
- Size: 9,999 movies
- Features: title, genre, language, overview, popularity, release date, vote average, vote count
## Tools & Technologies
- Python
- Pandas, NumPy
- Scikit-learn (CountVectorizer, Cosine Similarity)
- Google Colab
## Approach
- Preprocess movie tags (combine genres, keywords, overview).
- Convert text into numerical vectors using CountVectorizer.
- Compute similarity scores using Cosine Similarity.
- Recommend top 5 most similar movies.
## Example Recommendation
Input: "Iron Man"
Output:
- Iron Man  
- Mazinger Z: Infinity  
- Justice League Dark  
- Iron Man 3  
- The Colony  
## Results
- The system successfully recommends movies with similar genres and descriptions.
- Demonstrates how cosine similarity can capture relationships between superhero and action films.

