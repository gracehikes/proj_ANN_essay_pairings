
# Abstract
For popular dating apps and websites like Tinder, Bumble, Match and OKCupid, their
customer base ranges between two to eight million people. These companies employ a variety
of filtering, ranking and search algorithms in order to make match recommendations to their
users.

It is seldom done with brute computation force across all possible pairings or combinations. Let us use an example of a dating app with a customer base of four million users,
split 50/50 between men and women. If the dating company was interested in searching for
the closest matching essay embeddings for its users aged 20 to 29 years old, this narrows the
field down to say one million men and one million women. The number of possible pair-wise
comparisons that would have to be computed is one million times one million, or over one
trillion!


# Methodology
Instead a common technique used that makes embedding comparisons more efficient is
called Approximate Nearest Neighbors or ANN. Given a customer’s self-summary essay or
”subject essay” and the position of its embedding in the high-dimensional space, ANN will
search for other essay whose embeddings are mapped closer to this subject essay.

My analysis scope:
* apply ANN algorithm to dating app users' self-summary essays to get high-dimensional embeddings
* select two daters’ essays from the OkCupid data set and put them through the ANN
search algorithm
* read and validate top 3 closest essays

<p align="center">
  <img src="https://github.com/gracehikes/proj_dating_essays_tSNE_clusters/blob/main/images/essay%20lengths%2030%2070%20140%20example.png" width=70%>
</p>


# Results
It appeared men and women write in very similar manner for their dating self-summaries - see visualizations below. There were no clear clusters to be visualized by age of the dating singles. For pet preference, I also did not see separate clusters for dog-lovers versus cat-lovers. 

The longer the essay snippets used to generate embeddings, the closer the visualized data points start to merge to one another as shown in the diagrams below. The ability to see clusters (if any) favored shorter essay lengths.

<p align="center">
  <img src="https://github.com/gracehikes/proj_dating_essays_tSNE_clusters/blob/main/images/tSNE%20visual%20cluster%20by%20gender.png" width=95%>
</p>


# More Details
Full report found [here](/graceyang_final_thesis_filed.pdf).

