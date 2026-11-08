# Data-Science-Recommendation-System

This project builds several types of recommendation systems using real user–article interaction data from the IBM Watson Studio platform. It explores rank-based recommendations, collaborative filtering, content-based recommendations using NLP, and matrix factorization techniques to create personalized article suggestions.

## Prerequisites

Python 3.10 or higher (developed with 3.12)

Use the following Python packages in a Jupyter Notebook environment to complete the code portion of this project:  
- scikit-learn
- numpy
- pandas
- seaborn
- matplotlib

Files:
- `Recommendations_with_IBM.ipynb`
- `data\user-item-interactions.csv` - article interaction data
- `project_tests.py` - python tests
- `top_5.p` - .pickle files related to python tests
- `top_10.p`
- `top_20.p`

### Project Overview

This project explores and analyze the interactions that users have with articles on the IBM Watson Studio platform and make recommendations to them about new articles you think they will like.

Recommendation techniques explored in this project:  
- Rank-based: the most popular articles, best used for new users who have not had any interactions.  
- User-user collaborative filtering: articles read by the most similar users. Ties are broken by user activity and article popularity.  
- Content-based: TF-IDF + LSA on the article titles, KMeans with 50 clusters, and the most popular articles from the same cluster.  
- Matrix factorisation: SVD of the binary user-item matrix with 200 latent features, and article-article similarity in the latent space.  

---------------------------------
### License
- [License](https://github.com/danielzbarnes/data-science-recommendation-system/blob/main/LICENSE) GNU General Public License v3.0
