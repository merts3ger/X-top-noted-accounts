# X-top-noted-accounts
In this project, I conduct an analysis of X (Twitter) accounts that are most frequently flagged by Community Notes, a feature on X allowing the community to add context to and highlight incorrect information in tweets they believe are misleading.        
Given that these days social media play a big role in information warfare, it's important to keep exploring the problem of misinformation spread to effectively counteract its influence on public opinion.    
    
* Data collection involved web scraping and API requests: I used **Selenium** to get the current top "noted" accounts from the [leaderboards](https://community-notes-leaderboard.com/), capturing usernames, URLs, and note counts. Detailed user information and tweet metrics were retrieved using the **Tweepy** library via the Twitter API.     
* Next I looked into *user engagement* with these accounts, focusing on average retweets, likes, and follower counts.      
* **Topic modeling** with BERTopic was conducted to identify the most prevalent themes among these accounts.      
    * Data preparation involved removing URLs and account mentions, filtering out stop-words, and applying tokenization and lemmatization.      
    * *BERTweet* was selected as the embedding model because it is specifically trained on a large corpus of English tweets.        
* **Sentiment** analysis was performed using VADER.     

The analysis revealed that accounts marked for misinformation discuss sensitive topics, which at the time were the Gaza conflict and the legal case involving Jeffrey Epstein. Notably, some accounts demonstrated substantial engagement metrics, indicating huge resonance with readers. However, this project per its design did not consider the potential influence of social bots, which could significantly skew the metrics if active.
