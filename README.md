# Project: Book-Recommendation-System using Machine Learning!! | Collaborative Filtering Based
<img src="https://www.analyticssteps.com/backend/media/thumbnail/1658566/349446_1572064241_Banner1_Recommendation_System.jpg" alt="workflow" width="80%">
Recommendation systems have become pervasive and are used in a wide range of applications,
including e-commerce, social media, music and video streaming services, and of course, 
book recommendation systems. The rise of big data and machine learning has made it possible to 
process and analyze vast amounts of user data, leading to more accurate and personalized 
recommendations.
The purpose of a recommendation systems is to search for content that would be interesting 
to an individual. Moreover, it involves a number of factors to create personalised lists of 
useful and interesting content specific to each user/individual. Recommendation systems 
are Artificial Intelligence based algorithms that skim through all possible options and 
create a customized list of items that are interesting and relevant to an individual.
These results are based on their profile, search/browsing history, what other people 
with similar traits/demographics are watching, and how likely are you to watch those movies.
This is achieved through predictive modeling and heuristics with the data available.


# Types of Recommendation Systems :

### 1 ) Content Based :

- Content-based systems, which use characteristic information and takes item attriubutes into consideration .

- Twitter , Youtube .

- Which music you are listening , what singer are you watching . Form embeddings for the features .
	
- User specific actions or similar items reccomendation .
	
- It will create a vector of it .
	
- These systems make recommendations using a user's item and profile features. They hypothesize that if a user was interested in an item in the past, they will once again be interested in it in the future
	
- One issue that arises is making obvious recommendations because of excessive specialization (user A is only interested in categories B, C, and D, and the system is not able to recommend items outside those categories, even though they could be interesting to them).

### 2 ) Collaborative Based :
		
- Collaborative filtering systems, which are based on user-item interactions.
	
- Clusters of users with same ratings , similar users .
	
- Book recommendation , so use cluster mechanism .
	
- We take only one parameter , ratings or comments .
	
- In short, collaborative filtering systems are based on the assumption that if a user likes item A and another user likes the same item A as well as another item, item B, the first user could also be interested in the second item . 
	
- Issues are :

	- User-Item nXn matrix , so computationally expensive .

	- Only famous items will get reccomended .

	- New items might not get reccomended at all .   

### 3 ) Hybrid Based :
	
- Hybrid systems, which combine both types of information with the aim of avoiding problems that are generated when working with just one kind.

- Combination of both and used now a days .

- Uses : word2vec , embedding .   
     
# About the project:
This is a streamlit web application that can recommend various kinds of similar books based on the user interest.

# Data set:
*[Dataset link](https://www.kaggle.com/ra4u12/bookrecommendation)

# Concept used to build the model.pkl file : NearestNeighbors

1 . Load the data
	
2 . Initialise the value of k

3 . For getting the predicted class, iterate from 1 to total number of training data points

4 . Calculate the distance between test data and each row of training data. Here we will use Euclidean distance as our distance metric since it’s the most popular method. 

5 . Sort the calculated distances in ascending order based on distance values
	
6 . Get top k rows from the sorted array

# How to run ?
### Steps:

Clone the repository 
```cmd
https://github.com/Yasaswini-6304/Book-Recommender-System/
```
### STEP 01- Create a environment after opening the repository

```cmd
python m venv environment_name(env)
```

```cmd
env/Scripts/activate
```


### STEP 02- install the requirements
```cmd
pip install -r requirements.txt
```


```cmd
#run this file to generate the models

book_recommendation_system.ipynb
```

Now run,
```cmd
streamlit run app.py
```



