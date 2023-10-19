# Recommendations with IBM 
For this project, we have utilized interactions between users and articles on the IBM Watson Studio Platform. The goal of this project was to make recommendations to existing, 
and new users about articles they may like. 

First and foremost we go through various tasks to accomplish the recommendations provided to the user.

Description of Files:
  - Recommendations_with_IBM.ipynb : Jupyter Notebook where most of the following tasks are performed and recommendations are created
  - project_tests.py : File containing test code to ensure our methods are performed correctly.
  - rec_venv: virtual environment created for our Jupyter notebook
  - data: holds article_community data and user-item interactions that are captured during interactions with the IBM studio platform

1. Exploratory Data analysis section: We take a look at the data we will be working with from the IBM studio platform 
2. Rank-Based Recommendations: Our first recommendation for our users will be based on ranking articles. Since the articles
 themselves are not ranked, we will be utilizing counts of user interactions with specific articles. The more views an article contains
 the more popular that article is considered.
3. User-User-Based Collaborative Filtering: Ranking-based recommendations may not provide the best method for user recommendations.
 Articles may be viewed based on initial interests and not necessarily if the user enjoyed the article or not. Instead, we can find
users who enjoyed the same types of articles and find similar users to them and provide new articles the other users have read.
4. Matrix Factorization: Lastly, we utilize matrix factorization or SVD to create user recommendations. Using the user-item interactions,
   we can decompose the matrix to include its latent features and utilize this decomposition to predict new articles an individual may
   interact with.

   
For reviewers: snippet of code test running correctly
![Screen Shot 2023-10-19 at 2 43 30 PM](https://github.com/aurora-nat/ibm_recommendation_system/assets/67852929/ae19a330-292a-4bce-88fb-46a8c722f490)

