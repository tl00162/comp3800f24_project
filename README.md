# comp3800f24_project
Analyzed Twitter data to explore trends, sentiment, and engagement metrics about ai over time.

## Jupyter Notebook
The analysis and code are available in comp3800f24_project.ipynb

## Data

**Data Collection: ** Apify was utilized to scrape tweets from platform X due to its robust and customizable scraping capabilities, enabling the extraction of targeted data. The process focused on 177 unique hashtags and keywords, yielding 57,152 unique tweets. The total cost of this data collection effort was $78.12, covering API usage and computational resources. 

**Dataset Used:** The dataset consists of 57,152 unique tweets collected using the 177 hashtags and keywords related to ai. 
The keywords used for scraping can be found in the keywords.csv file included in this repository.
The total size of the dataset csv is approximately 26 MB

**Preprocessing:** 
Basic preprocessing steps were applied, including:

Removing duplicate tweets to ensure uniqueness.
Cleaning hashtags and keywords to avoid noise in the dataset.
Standardizing text data

This cleaned dataset forms the foundation for further analysis and visualization.
 
 ## Results
### Key Insights
1. I hypothesized that highly positive and negative tweets would yield the highest levels of engagement. To visualize this, I split the tweets into groups based on neutral sentiment -.5<x<.5 and highly negative and positve sentiment.   All three groups had a similar number of replies, however the highly negative tweets saw a over double the amount of likes and qutoes with nearly double the retweets and views on average compared to the neutral and highly positive tweets. The hypothesis was close to correct, but the results show the best way to be engaged with on X is negative sentiment tweets.  The positive tweets did slightly worse than neutral across the board. 
2. I predicted NFT would be the most negatively recieved keyword we filtered for, this was shown to be incorrect. Highly negative NFT tweets performed much worse on average than neutral or even positive tweets on the subject.  This could be due to a feedback loop where the majority of people engaging with NFT-related tweets are entrenched supporters or enthusiasts of the topic, leading to a self-reinforcing echo chamber that amplifies positive or neutral sentiment while deterring widespread criticism or engagement from detractors.

### Visualizations
Here are some key visualizations from the project:

#### Plot 1:  A bar plot showing the 20 most frequently occuring stems from the tweets. There was an emphasis on ai, transparency and trust.
[Plot 1](images/plot1.png)

#### Plot 2: Word Cloud of All Tweets: Similar to the most frequent stems, the word cloud highlights the importance of transparency and trust in ai.
[Plot 2](images/plot2.png)

#### Plot 3: Word Cloud of Top Positive Tweets: The positive tweets have stems about the best uses for ai, how it is great at creating images.
[Plot 3](images/plot3.png)

#### Plot 4: Word Cloud of Top Negative Tweets: The negative tweets focus heavily on trust and user rights.
[Plot 4](images/plot4.png)

#### Plot 5: Sentiment Over Time: Sentiment of ai started much more volatile before 2021, when it was less understood. Starting in 2021 and especially after twitter changed to X there has been overall slight positive sentiment towards ai.
[Plot 5](images/plot5.png)

#### Plot 6: Engagement by Polarization (All Keywords) : Box plots showing that negative sentiment tweets are likely to have normal reply counts but higher views, quotes, likes, and retweets on average compared to neutral or positive tweets.
[Plot 6](images/plot6.png)

#### Plot 7: Engagement by Polarization (NFT Tweets Only): Surprisingly there were not many popular highly negative tweets about nfts. One reason mayy be anyone tweeting about them did so from a place of understanding.
[Plot 7](images/plot7.png)




## How to Run
- Clone the repository: git clone https://github.com/yourusername/yourrepository-name.git
- Install dependencies: pip install -r requirements.txt
Open the notebook: jupyter notebook comp3800f24_project.ipynb