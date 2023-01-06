# Amazon-Product-Recommender-System

Performed sentiment analysis on Amazon Review Dataset available at http://snap.stanford.edu/data/web-Amazon.html

# Introduction to Recommendation systems

In this modern world we are overloaded with data and this data provides us the useful information. But it's not possible for the user to extract the information which interest them from these data. In order to help the user to find out information about the product , recommedation systems where required. 

Online shopping is all over the internet. All our needs are just a click away. The biggest online shopping website is Amazon. Amazon is known not only for its variety of products but also for its strong recommendation system.     

In our project we are taking into consideration the amazon review dataset for Clothes, shoes and jewelleries and Beauty products. We are considering the reviews and ratings given by the user to different products as well as his/her reviews about his/her experience with the product(s).  

Recommeder system creates a similarity between the user and items and exploits the similarity between user/item to make recommendations.

Based on these input factors, sentiment analysis is performed on predicting the helpfulness of the reviews. 
Moreover, we also designed item-based collaborative filtering model based on k-Nearest Neighbors to find the 2 most similar items.     

# What recommeder system can solve ?

1. It can help the user to find the right product.
2. It can increase the user engagement. For example, there's 40% more click on the google news due to recommendation.
3. It helps the item providers to deliver the items to the right user.In Amazon , 35 % products get sold due to recommendation.
4. It helps to make the contents more personalized.In Netflix most of the rented movies are from recommendations.

# Types of recommendations

There are mainly 6 types of the recommendations systems :-

1. Popularity based systems :- It works by recommeding items viewed and purchased by most people and are rated high.It is not a personalized recommendation.
2. Classification model based:- It works by understanding the features of the user and applying the classification algorithm to decide whether the user is     interested or not in the prodcut.
3. Content based recommedations:- It is based on the information on the contents of the item rather than on the user opinions.The main idea is if the user likes an item then he or she will like the "other" similar item.
4. Collaberative Filtering:- It is based on assumption that people like things similar to other things they like, and things that are liked by other people with similar taste. it is mainly of two types:
 a) User-User 
 b) Item -Item
 
5. Hybrid Approaches:- This system approach is to combine collaborative filtering, content-based filtering, and other approaches . 
6. Association rule mining :- Association rules capture the relationships between items based on their patterns of co-occurrence across transactions.

# Learning Outcomes:  
Amazon to provide different suggestions to different users. Amazon currently uses item-to-item collaborative filtering, which scales to massive data sets and produces high-quality recommendations in real-time.

#### ● Exploratory Data Analysis 
#### ● Creating a Recommendation system using real data 
#### ● Benchemarking Popularity based models, Matrix factorization model and Collaborative filtering 

# Data Description:  

Performed sentiment analysis on Amazon Review Dataset available at http://snap.stanford.edu/data/web-Amazon.html

Kaggle Dataset Link :  https://www.kaggle.com/saurav9786/amazon-product-reviews?fbclid=IwAR26xfJJK1c5zEeXh8yK9tTgDZrXSkdZIIfjGOhnegCobgskrUEYFcky_cw

The dataset here is taken from the below website.

Source - Amazon Reviews data (http://jmcauley.ucsd.edu/data/amazon/) The repository has several datasets. For this case study, we are using the Electronics dataset.



# Steps and tasks: 

#### 1. Read and explore the given dataset.  (Rename column/add headers, plot histograms, find data characteristics) 
#### 2. Take a subset of the dataset to make it less sparse/ denser. ( For example, keep the users only who has given 50 or more number of ratings )  
#### 3. Split the data randomly into train and test dataset. ( For example, split it in 70/30 ratio) 
#### 4. Build Popularity Recommender model.  
#### 5. Build Collaborative Filtering model. 
#### 6. Evaluate both the models. ( Once the model is trained on the training data, it can be used to compute the error (RMSE) on predictions made on the test data.  
#### 7. Get top - K ( K = 5) recommendations. Since our goal is to recommend new products for each user based on his/her habits, we will recommend 5 new products.  
#### 8. Summarise your insights. 


# Convert json to CSV using following commands
```
dataframe = pd.read_json('reviews.json')
dataframe.to_csv('reviews.csv', sep=',', index=False)
```
# Algorithms performed
## Sentiment analysis:    
1. [Logistic Regression](https://github.com/ayushete02/Amazon-Product-Recommender-System/tree/main/Logistic%20Regression)    
2. [Naive Bayes - Multinomial and Bernoulli](https://github.com/ayushete02/Amazon-Product-Recommender-System/tree/main/Naive%20Bayes)    
3. [LSTM](https://github.com/ayushete02/Amazon-Product-Recommender-System/tree/main/LSTM)    
    
# Recommender system:    
k-Nearest Neighbors is used to perform [item-based collaborative filtering](https://github.com/ayushete02/Amazon-Product-Recommender-System/tree/main/Recommender%20System)    
    
# Contibutions    
1. Khushi Gaidhane
2. Ayush Shete 
        
# References:    
1. [J. McAuley and J. Leskovec. Hidden factors and hidden topics: understanding rating dimensions with review text. RecSys, 2013.](http://i.stanford.edu/~julian/pdfs/recsys13.pdf)    
2. http://jmcauley.ucsd.edu/data/amazon/    
3. https://www.kaggle.com/snap/amazon-fine-food-reviews   
