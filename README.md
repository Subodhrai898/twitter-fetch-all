# twitter-fetch-all
Python script to fetch all the tweets of the user from his/her timeline.This script which can fetch all the tweets  and dump the responses into JSONlines file.
 
 The other part of this script should be able to parse these JSONline files to display the
 following for every tweet in a tabular format.
● The text of the tweet.
● Date and time of the tweet.(Used as Index)
● The number of favorites/likes.
● The number of retweets.
● Number of Images present in Tweet. If no image returns None.

Modules required
<ol>
 <li>Pandas</li>
 <li>Jsonlines</li>
 <li>Tweepy</li>
 <li>Datetime</li>
</ol>

Here,I<br>
Use Tweepy module for twitter API<br>
Use Jsonline module to dump all tweets in .jsonl file<br>
Function used here get_tweets() for getting list of tweets<br>
Use Pandas Dataframes to show and store data in tabular form<br>
<br>
get_tweets is our main function which call Rest Api of twitter and api.user_timeline used to fetch all the tweets.
Here I used loop which extract tweet in bunch of 200 tweets at one time untill in next iteration we will not get any tweets.
I also used extended mode to get all information of the tweet including images details and full text.
<br>
Function used
<ol>
 <li>get_tweets</li>
 <li>store_jsonl</li>
 <li>Create_DataFrame</li>
 <li>jsonl_to_dataframe</li>
</ol>
<br>
Here I used Pandas Dataframe to show and store data in Tabular from.Dataframes have columns Text , Like , Retweet_Count ,Number of Image.Here I used Datetime as index and create a Time Series.The benefit of Time Series Data is that we can easily analyse it.




"Please Read Comments to understand the code"
