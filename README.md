Movie Recommendation System


This project uses a content-based movie recommendation system that recommends movies based on their metadata (tags, genres, keywords, etc.).


How It Works

1.Text Vectorization
We extract features from the descriptive tags of each movie using Bag-of-Words with CountVectorizer
max_features=5000
English stop word removal for better representation

2.Cosine Similarity Calculation
We transform the tag matrix to vector form and calculate pairwise cosine similarity between movies using

3.Ranking & Recommendations
Given a movie, the system:
Finds the closest movies in cosine space
Ranks them according to similarity score
Returns Top 5 Recommendations (essentially a k-NN search in vector space)

Key Highlights


-No collaborative filtering (purely content based)

-Scalable to thousands of movies with efficient vectorization

-Lightweight and easy to integrate with any movie datase


Technologies Used
Python 3.x

scikit-learn – for vectorization & similarity computation

pandas – for dataset handling

numpy – for numerical operations
