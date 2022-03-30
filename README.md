
# Abstract
For popular dating apps and websites like Tinder, Bumble, Match and OKCupid, their customer base ranges between two to eight million people. These companies employ a variety of filtering, ranking and search algorithms to make match recommendations to their users quickly.

Matching of similarity is not done with brute computation force across all possible pairings or combinations; there is a business need to compute efficiently and produce speedy match recommendations between the millions of dating app users. Instead, tech companies make use of an approximate matching algorithm to find neighbor matches in the blink of an eye with only very small sacrifices in accuracy.


# Methodology
A common algorithm used to make embedding comparisons more efficient is Approximate Nearest Neighbors (ANN). Given a dating app user’s self-summary and the position of its embedding in the high-dimensional space, ANN can rank other essays whose embeddings are mapped close to this subject essay.

My analysis scope:
* apply Google's TensorFlow Hub (TF-Hub) model to dating essays to get high-dimensional embeddings
* build an ANN ranking of essay similarity or "proximity" with embeddings generated from TF-Hub model
* use the ANN ranking to find most similar essay matches
* put dating app users’ essays through the TF-Hub embedding and ANN ranking, check and validate top 3 essay "matches"

<p align="center">
  <img src="https://github.com/gracehikes/proj_dating_essays_tSNE_clusters/blob/main/images/essay%20lengths%2030%2070%20140%20example.png" width=70%>
</p>


# Results
Let's review a sample essay and its 3 closest ANN-ranked matches out of the 60,000+ essays. The high-dimensional embeddings appeared to have done a good job of capturing the essense in the sample essay--moving to different states for school/work, a hobby of international travel, possessing advanced educational degrees--and finding similar matches.

<p align="center">
  <img src="https://github.com/gracehikes/proj_dating_essays_tSNE_clusters/blob/main/images/tSNE%20visual%20cluster%20by%20gender.png" width=95%>
</p>


# More Details
Full report found [here](/graceyang_final_thesis_filed.pdf).

