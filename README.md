# PlayStoreAppAnalysis

Visual Exploration Tool
------------------------

Title: 
Google Play Store App Rating Analysis
---------------------------------------

This is an adaptation of the play store apps dataset provided by Kaggle. The original dataset provides details of 10K Play Store apps for analysing the android market. Features on apps available include the Category, Rating, Number of Reviews, Installs, Type, Content Rating, Genres, Review, Sentiment, Polarity, Subjectivity. The original dataset provides application data of number of categories and content rating. It also provides application review data with its sentiment value. I used Python to derive a new version of this dataset where I have merged both the application detail dataset and application review dataset. I modified the sentiment attribute of the nominal type to quantitative type through a simple mapping of -1 for Negative, 0 for Neutral and +1 for Positive. This was simply summarised as mean sentiment value for each application.

My overall goal with this tool was to enable the exploration of the relationship between the sentiment of app reviews (Sentiment), the rating these applications received (Rating), and how this varies for different categories/genres and content rating.


Cross-filtering is the primary method of engagement that I have employed in this case. Users may filter data in another chart by selecting subsets of the data in one chart, e.g. users can select only one category in the bar-chart and this will filter the data presented in both the histogram and the scatter-plot. Each chart enables selection on a different data attribute – the bar chart allows selection by category, the histogram allows selection based on application rating range, the scatter plot allows selection of applications belonging to certain sentiment area. There is an interactive legend at the top to allow selection based on content rating type. Combination of these interactions allow the user to explore the relationship between different attributes – e.g. what are the highly rated categories? Which content rating most follows the sentiment – rating relationship? How are categories distributed for each content rating? 
