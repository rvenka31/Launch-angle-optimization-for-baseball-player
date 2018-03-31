# Launch-angle-optimization-for-baseball-player

Introduction:
This is a part of the case competition conducted by SABR (Society for American Baseball Research) during March 9 to 11.
We needed to optimize the launch angle for 3 players. We implemented our procedure in ML AZURE. The results weren't satisfactory due to an error in our approach. I have corrected it and implemented the logic in Python. I have choosen Jackie Bradley Jr of Boston Red Sox. We have used the data avaiable from https://baseballsavant.mlb.com/ for our analysis. I thank my team mates in this case for their support and knowledge sharing.


Approach:
1.We collected the data from 2015-2017 for all batted balls for all players. 
2.We identified peer groups for each player by implementing recommendation system principle using Euclidean distance measure to identify similar players based upon the physical traits. We ranked them based on performance metrics and choose the top 30 players.
3.For Jackie Bradley Jr. we looked at his peer group and we created the training dataset based upon his peer group. 
4.I trained our model to predict the outcome of a pitch based upon the data of the peer group instead of the entire player pool which was our approach before using ML AZURE.
5.I have tried different algorithms & Hyperparameter tunning and selected the models with best Accuracy measure.
6.I used Majority voting to determing the final outcome. 

Results:

Outcome	    No.of times
Out	        6735
SINGLE	    3672
DOUBLE	    220
TRIPLE	    0
HR	        233
Total       10860


