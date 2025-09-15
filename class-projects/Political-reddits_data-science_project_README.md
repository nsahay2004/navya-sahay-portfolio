(cannot be shared due to university privacy regions. ) 
Project Description:

This project sets out to analyze the relationships between political and non-political communities on Reddit using a variety of different data analysis techniques. 
We have three primary hypotheses we tested using statistical methods such as a two-sample T-test and linear regression. 
Our research hypotheses are as follows:

Hypothesis A: There is a positive correlation between the distance from a political community and the negative sentiments of those communities.
Hypothesis B: Republican connected subreddits have a more positive sentiment than Democrat connected subreddits.
Hypothesis C: There is a negative correlation between the distance between two nodes and how politically biased they are.

To answer these hypotheses we used an automated script that interacted with Reddit’s API through the Python Reddit API Wrapper (PRAW) to 
collect a large sample of user-generated content from different communities. Our strategy revolved around using a careful selection of 
“seed communities” that included some of the most political liberal and conservative subreddits. For each of these communities our algorithm 
first obtained a representative sample of the community by collecting the names of the authors of the top posts over the past year, month, week, 
and day. If over 5 of these top authors also had top or recent posts/comments in another community that subreddit was then added to a queue for analysis. 
By crawling in this automated manner our data grew organically without researcher bias and gave us a large sample.

My main contribution: 
To address our last hypothesis we used a transformer-based BERT model to determine how left, center, and right each post was in the different 
communities. We used the ratio of left to right to get a political score. The lesser the score was the more right the text was and the higher the 
score/ratio was the more left the text was. We used a linear regression model to determine if there was a correlation between distance from the root 
nodes and the sentiment score. The mean squared error we got was 3926.62 which given the scale of the political bias ratio (with the maximum political 
bias being approximately 550 indicating extreme bias towards left) was relatively low, indicating a reasonably high accuracy. We got a p_value of
0.034 <= 0.05. Hence, we can reject the null hypothesis that there is no correlation between the two variables as the low p_value indicates 
statistical significance for the correlation. As we got a correlation slope of -1.6686, it suggests a negative correlation.  However, the R2 value 
was 0.0019 which is very low and suggests that this correlation has little variance and is not necessarily the best predictive model for the relationship 
between the two variables. 
