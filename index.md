<div style="text-align: justify"> Sparkify is a fictional popular music streaming service similar to Spotify. The objective of the project is to forecast churn of the platform users. The dataset provided contains detailed information on events of users behavoiur on the platform, including among others the page they are on, the music they listen (artist, song title), users location and timestamp. The data analysis and modelling were programmed in PySpark. The link to Jupyter Notebook is provided in the References. </div> 

The article covers the following parts:
1. Data Description
2. Feature Engineering
3. Modeling
4. Summary

#### 1. Data Description
The dataset consists of 286500 rows and 18 columns. The description of the columns is as following:
* **artist** - name of the artist if user's page is *NextSong*, Null otherwise
* **auth** - has two categories *Logged In* or *Cancelled*
* **firstName** - first name of the user
* **gender** - gender of the user. Two categories: F (female), M (male)
* **itemInSession** - indicates the order of user's event during a session
* **lastName** - last name of the user
* **length** - length of the song in seconds if user's page is *NextSong*, Null otherwise
* **level** - *paid* or *free*, distinguishing free and paid users
* **location** - geographical location of the user
* **method** - takes two values: *PUT* or *GET*
* **page** - represents the event on Sparkify. Have 19 unique categories
* **registration** - registration time of each user
* **sessionId** - numerical Id of user's session. One user can have multiple sessions
* **song** - song name
* **status** - HTTP status codes
* **ts** - timestamp of the event
* **userAgent** - the user-Agent used 
* **userId** - unique user identifier

<div style="text-align: justify"> To create ML model for customer churn, the churn must be defined.
When user goes to page Cancellation Confirmation he quits and there are no more records for the user after this event.
Therefore the Cancellation Confirmation page is used to define Churn label. </div> 

#### 2. Feature Engineering
After detailed data analysis (see Jupyter Notebook for details), the following features are proposed:
* **male** - representing 1 for males, 0 for females. In historical data males proportionally more often churn
* **artists_count** - representing number of distinct artists listened by a particular user. In historical data users with higher number of uniqe artists less often churn
* **avg_session_items** - representing average number of items per user's session. In historical data users with higher number of session items less often churn
* **date_diff** - representing the period of time in days since user uses Sparkify

#### 3. Modeling
Two machine learning models are used in this supervised learning classification problem. Namely, logistic regression and random forests. The data is split to train and test in the proportion of 70% and 30% accordingly. As the dataset is unbalanced, because 23% of users churn, we will use F1-score as the main optimization metric. The F1-score presents the model’s balanced ability to both capture positive cases (recall) and be accurate with the cases it does capture (precision).
The score of logistic regression is 75%, whereas of random forests 77 %. F1-score of about 80% indicates that the model performance on unseen data is very good.

#### 4. Summary
From the business perspective knowing if customer is going to churn before he or she does it is a very valuable information. The company can act accordingly to keep the customers, before they leave. In this study two machine learning models were run. Random Forest provides a bit better results according to F1-score. The model categorizes the customers correctly in 80% cases, which is a very good performance and can bring significant busines value.
The following improvements can be made to enhance the results:
* develop new features. For example a good candidate is a *page* column representing 19 events. Occurence of some of those events might indicate user behaviour that helps predicting its' churn.
* try other machine learning models. For example Gradient-boosted trees, SVMs.
* check for optimal hyperparameters for the currently checked and new models.

#### References
[Jupyter Notebook based on which this article was created](https://github.com/Pawelwl/sparkify-churn-prediction/blob/main/Sparkify.ipynb) <br>
