# Recommendation-System
Movie recommendation system to suggest new movies for users.

For this project, we will use the MovieLens latest dataset available on grouplens.org. The dataset consists of multiple .csv files. Different files contain different attributes such as movieID, userID, movie-name, genre, ratings, tags, genome tags, relevance scores, etc. These data were created by 610 different users and contains 100836 ratings with 3683 tag applications across 9742 different movies. 
This data can is publically available and can be found at - https://grouplens.org/datasets/movielens/
The subset of the data that I have used for this project is included in this repository.

There two ways to create a recommendation system - Collaborative filtering and Content based filtering approach.

Collaborative filtering further has 3 more types of implementaions - Item - Item Collaborative filtering, User - User Collaborative filtering and Item - User Collaborative filtering. In this project, I have created a recommendation system using Item - Item Collaborative filtering and User - User Collaborative filtering approaches.

In Item - Item Collaborative filtering, we try to find items (in this scenario, movies) that are very similar to the items that a particular user has already purchased in the passed (in this scenario, watched). The items that are highly similar to the ones already bought and like by the user are recommended by the system. This similarity between the items is calculated by find correlation amongst the items. The metrics used for this is the ratings given by the user to every movie it has watched.

User - User Collaborative filtering, we try to find users that are similar to the user under consideration, to whom we want to make recommendations. These similarities are found on the basis of buying pattern or like in our case, ratings given to a product using correlation. Then the user is recommended the items are most liked by the users that are very similar to him/her.

Here, I have made a few assumptions. The first assumption is that the movies liked by a user are rated more than 4 on a scale of 5 and a correlation value more than 0.95 indicates high similarity. 
