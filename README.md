# Describing Political Diversity in Reddit Communities using GS-scores

## Abstract
GS-score, calculated as the average cosine similarity between its communities and its center of mass, is a well-defined metric for a user’s activity diversity. In the reference paper, the analysis is conducted on the entire Reddit dataset using GS-score. The process could also be applied to a specific subset, namely the one of political subreddits, and different interpretations can be generated as opposed to the process on the whole dataset - the GS-score now becomes a measure of a user’s political diversity. We are interested in the general distribution of users’ GS-scores. Also, we try to analyze how likely users are to stay in a community after their first contribution. Moreover, user’s parent-universe is the population it interacts with; the relationship between the GS-score of its parent-universe and of its own can now be used to detect political echo chambers.

## Research questions
1.	The distribution (frequency) of GS-scores over users active in political subreddits. (primary)
2.	How likely are users to stay engaged in the subreddits after a certain time period they’ve joined?
3.	How does the GS-score of a user correlate to the GS-score of its parent-universe?

## Methods
The attention should be focused on only users who are active in at least 1 political subreddits. The subset of political communities can be formed by manually identifying political subreddits (after exploring the dataset, there are only 92 distinctive subreddits; manual identification is then quick and accurate)
1.	With the processed data, calculate GS-score for all users and store it in a new column. GS-score is defined as the average cosine similarity between its communities and its center of mass. The plot of the GS-score distribution can be broken down by number of communities with range specified.
2.	Examine all the occurrences of when users join a new community, and then calculate the probability that they are still engaged in the community after a certain period (6 months). Draw a line plot to see how does the probability change along with the magnitude of the GS-score. Compare the probability of generalists and specialists.
3.	Define parent-universe as the set of users that a user replied to. Calculate the average GS-score of all users’ parent-universe. Plot the distribution of the parent universe GS-scores as a function of user GS-score with a box plot.
