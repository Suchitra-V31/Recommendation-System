**Recommendation-System**

Recommender systems are an important class of machine learning algorithms that offer "relevant" suggestions to users. 
Categorized as either collaborative filtering or a content-based system.
How does YouTube know what videos you’ll watch? How does Google always seem to know what news you’ll read? They use a Machine Learning technique called **Recommender Systems**.

Practically, recommender systems encompass a class of techniques and algorithms which are able to suggest “relevant” items to users. Ideally, the suggested items are as relevant to the user as possible, so that the user can engage with those items: YouTube videos, news articles, online products, and so on.

Items are ranked according to their relevancy, and the most relevant ones are shown to the user. The relevancy is something that the recommender system must determine and is mainly based on historical data. If you’ve recently watched YouTube videos about elephants, then YouTube is going to start showing you a lot of elephant videos with similar titles and themes!

Recommender systems are generally divided into two main categories: **collaborative filtering and content-based systems**.

**Collaborative Filtering Systems**

Collaborative filtering methods for recommender systems are methods that are solely based on the past interactions between users and the target items. Thus, the input to a collaborative filtering system will be all historical data of user interactions with target items. This data is typically stored in a matrix where the rows are the users, and the columns are the items.

The core idea behind such systems is that the historical data of the users should be enough to make a prediction. I.e we don’t need anything more than that historical data, no extra push from the user, no presently trending information, etc
Beyond this, collaborative filtering methods are further divided into two sub-groups: **memory-based and model-based methods**.

**Memory-based methods** are the most simplistic as they use no model whatsoever. They assume that predictions can be made on pure “memory” of past data and usually just employ a simple distance-measurement approach, like nearest neighbour.

**Model-based approaches**, on the other hand, always assume some kind of underlying model and basically try to make sure that whatever predictions come out will fit the model well.

**Content-based Systems**

As an example, let’s say we have a matrix of users-to-preferred lunch item where all of the users are Americans who love cheeseburgers (they are phenomenal). A memory-based method will only look at what the user has eaten over the past month, without considering that mini-fact of them being cheeseburger loving Americans. A model-based method, on the other hand, will ensure that the predictions always lean a bit more towards being a cheeseburger, since the underlying model assumption is that most people in the dataset should love cheeseburgers!
In contrast to collaborative filtering, content-based approaches will use additional information about the user and / or items to make predictions.

For example, in the gif we saw above, a content-based system might consider the age, sex, occupation, and other personal user factors when making the predictions. It’s much easier to predict that the person wouldn’t like the video if we knew it was about skateboarding, but the user’s age is 87!
That’s why when you sign up for many online websites and services, they ask you to (optionally) give your date of birth, gender, and ethnicity! It’s just more data for their system to make better predictions.

Thus, content-based methods are more similar to classical machine learning, in the sense that we will build features based on user and item data and use that to help us make predictions. Our system input is then the features of the user and the features of the item. Our system output is the prediction of whether or not the user would like or dislike the item.
