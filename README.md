# Reddit Post Score

Link to Deployed Application : https://reddit-post-score.herokuapp.com/

### About the Project: <h3>
This project is about predicting the overall score a Reddit post will get. Score is the result of upvotes and downvotes for a particular post. The dataset was created using web scarpping with the help of praw library. The features exracted are:
*Title - title o fthe post
*Gilded - rewarding a Reddit gold to the post
*Over_18 - True if the post has adult content else False
*Ups - no of upvotes for the post
*Downs - no of downvotes for the post
*Num_of_comments - no of comments for the post
*Upvote_ratio - upvote ratio of the post
*Score - total score (upvotes - downvotes)
Later sentiment analysis was done using Vader Sentiment analyzer for the title field. We get 4 features pos, neg, neu and compund which tells how positive or negative the sentiment is. All these features were combined to form a single feature 'Predict_value' based on the compund score.

### Installing required librarires: <h3>
* Installing __keras__ and __tenserflow__:
```
pip install keras==2.2.4
pip install tensorflow==2.0
```
* Installing nltk:
```
import nltk
nltk.download('popular')
```
* Installing xgboost:
```
pip install xgboost
```
* Installing vaderSentiment:
```
pip install vaderSentiment
```
* Installing praw:
```
pip install praw
```
__Note__: Run these commands in the notebook that you are working.

Google Drive link for dataset (ScrappedPostsData.csv): https://drive.google.com/file/d/15nO0765lScyH17q-XvJ068hD7-spne0T/view?usp=sharing
