# Recommendation System for Microsoft's Launch into Video Streaming 
## Generating a Recommendation System with Hybrid Approach for Improved Accuracy in Predicting User Preferences in Video Content.

  ![IMG-4822](https://github.com/mahumabid/phase4-project/assets/122308796/4828780a-6a1d-4ee4-babb-b69a150c6c47)


Authors: Mahum Abid, Hera K.

Date: 05/12/2023

## Stakeholder: Netflix

![IMG-4823](https://github.com/mahumabid/phase4-project/assets/122308796/80ff2063-23c8-4dc5-8ad4-b85e013cade6)

## Project Overview
This project involves building a recommendation system for movies based on the MovieLens dataset, sourced from the GroupLens research lab at the University of Minnesota. The task at hand is to develop a model that can provide top 5 movie recommendations to users, based on their ratings of other movies. To accomplish this, the collaborative filtering approach must be implemented, and a potential hybrid approach could be explored by incorporating content-based filtering to address the cold start problem. The dataset is a widely-used recommendation system dataset in academic literature, and the project requires formulating a specific business problem within the context of recommending movies. Evaluation of the model can be done using the explicit ratings available in the dataset, and careful consideration of metrics is recommended.
## Recommendation System Overview
A recommendation system is a type of information filtering system that aims to predict a user's preference or rating for a particular item. These systems can be found in various areas such as movies, music, news, social tags, and products. Recommendation systems usually provide a list of recommendations to the user, and there are two popular methods to do this - collaborative filtering and content-based filtering.

Many popular internet products today, like YouTube, Netflix, Amazon, HBO, Peacock, and Disney rely heavily on recommendation systems to filter through millions of contents and provide personalized recommendations to their users. These systems have been extensively studied and proven to provide significant value to both businesses and consumers.

In the media and entertainment industry, there are six main types of recommendation systems. In this project we focused on collaborative, content-based, and hybrid for the launch of this new streaming platform. The concept of a recommendation system is quite broad, and various algorithms can be used to create such systems. The type of recommender system chosen depends largely on the type of available data. Below is a better description of each system.

![IMG-4824](https://github.com/mahumabid/phase4-project/assets/122308796/3f97a9f7-4315-4317-9c64-8e6dddba1651)


## Content-based Recommendation System:
This type of recommendation system uses specific characteristics or features of an item, such as its description, to suggest similar items to the user. It also takes into account the user's preferences and history to generate personalized recommendations. For example, it can recommend movies that are similar to a movie that the user has watched or based on all of the movies that the user has viewed. The system extracts relevant features from the item and uses the user's history to provide suggestions.
## Collaborative Recommendation System:
Collaborative filtering assumes that users who have agreed in the past are likely to agree in the future and have similar preferences. This method generates recommendations by analyzing the rating profiles of different users or items. By identifying other users/items with similar rating histories to the current user/item, it generates recommendations using this information. This technique creates a model based on a user's past actions, including items purchased, selected, or rated. The model is then used to predict items or ratings that the user may be interested in. Collaborative filtering can be classified as memory-based or model-based.
## Hybrid Recommendation System:
A hybrid recommender system combines multiple recommendation techniques to solve problems and improve accuracy. This approach can overcome common issues in recommender systems such as cold start, sparsity, and knowledge engineering bottlenecks. By integrating content-based and collaborative filtering techniques, the hybrid recommender system can leverage the strengths of both approaches and minimize their limitations. Research has shown that hybrid recommender systems perform better than pure content-based or collaborative filtering methods
## Recommendation System at Work:
The following includes results printed from our model for userId 2. We used the famous SVD algorithm and the surprise package to create, all of our models.Our Hybrid-Based Model combines both Collaborative and Content-Based models as well as offers our best predicted ratings compared to actual ratings of what your users would highly rate and watch.

## The Data

The MovieLens Latest Small dataset, which is a collection of ratings and metadata for a variety of movies. Here's a brief summary of the dataset:

- The MovieLens Latest Small dataset contains 100,000 ratings of 9,724 movies provided by 610 users.
- The ratings are on a scale of 1 to 5, in half-star increments(i.e. 0.5, 1.0, 1.5, etc.).
- In addition to the ratings, the dataset includes movie metadata such as titles, genres, and release years.
- The movies in the dataset come from a variety of genres, including drama, comedy, action, and romance.
- The dataset was collected between January 09, 1995 and October 16, 2016.
- The ratings in the dataset are fairly sparse, meaning that not every user rated every movie. In fact, there are many movies in the dataset that received only a handful of ratings, making it challenging to accurately predict their popularity.
- To address the cold-start problem, we created the content-based system. This ensures that old and new users will be recommended possible watches and help users continuously use our platform.
## Our Models
#### Our Super Users:

The dataset is skewed as certain users have contributed significantly more data than others. Specifically, two users who favored the drama genre made up almost 5% of the entire dataset. As a result, their preferences may have influenced their ratings for other genres, and they may have rated dramas and comedies higher due to their personal preference.

![top5_user474](https://github.com/mahumabid/phase4-project/assets/122308796/2f5c1de1-c51a-46fb-a328-f4572bd3ee81)
![top5_user414](https://github.com/mahumabid/phase4-project/assets/122308796/ccbda24d-21ff-4b9f-b631-a22658f90f4e)




#### Ratings by Top 100 Users:

The distribution of ratings in the dataset is heavily skewed towards positive ratings. About 60% of the ratings are 4 stars or higher, which indicates that users in the dataset generally enjoyed the movies they watched.

![top100](https://github.com/mahumabid/phase4-project/assets/122308796/a13bf2bf-71a0-45ac-a521-843b76df6b03)


#### Average viewers by Top 10 Genres:

The data limitations have caused a skew in the number of views for each genre. Although documentaries may not be the most popular genre, we believe that with sufficient data from a diverse set of users, it could gain popularity.

![AvgNumViews_Genre](https://github.com/mahumabid/phase4-project/assets/122308796/826fe174-1878-4445-8fb9-6e0c27710131)


## Conclusion

The dataset includes a wide variety of movies, ranging from obscure independent films to popular blockbusters. However, the most frequently rated movies tend to be well-known classics, such as "Forrest Gump", "Pulp Fiction", and "The Shawshank Redemption". Researchers have used the MovieLens dataset to explore a wide range of topics in recommendation systems, such as collaborative filtering, content-based filtering, and hybrid approaches. The dataset has also been used to evaluate the performance of various machine learning algorithms and to test the effectiveness of different recommendation strategies.
## Structure

This is the README of the project. The repo contains our technical jupyter notebook (Final-Notebook.ipynb) which shows the code used to prepare, clean, and model the data. Our final non-technical presentation can be seen at presentation.pdf
