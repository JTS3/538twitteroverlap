# A Brief Note on 538 Twitter Overlap


In this [data journalism piece](https://fivethirtyeight.com/features/which-2020-candidates-have-the-most-in-common-on-twitter/) by Gus Wezerek [@guswez](https://twitter.com/guswez) or and Oliver Roeder [@ollie](https://twitter.com/ollie),  the authors do not note that lift is a function of the number of followers.  

The larger a candidate's twitter following the more isolated that following tends to be. The authors present the data as a table but it helps to plot the candidate's exclusive following against the size of their following. 

![alt text](https://github.com/JTS3/538twitteroverlap/blob/master/sharedbytwo_exclusivefollowers_followers.png "Exclusive Followers v Followers")

Williamson's following's isolation stands out relative to her following's size; her name is high above the OLS line.  To a lesser extent we see the same kind of isolation happening with Hickenlooper, Yang, and Gabbard.  Wezerek and Roeder note Warren's followers gregariousness; they are far below the OLS line.  A similar thing could be said of Swalwell, did you know that 72% of Swalwell fans also follow Harris? 

Wezerek and Roeder use lift to get at the independence of a candidate's following.  Below, I plot log(lift) against log(followers). When log(lift) is zero, then lift is one and the events are independent.  When log(lift) is below zero, then sharing a follower is less likely than if you assumed following was independent. When log(lift) is above zero, then sharing a follower is more likely than if you assumed independence. 

![alt text](https://github.com/JTS3/538twitteroverlap/blob/master/sharedbytwo_loglift_logfollowers.png "Lift v Followers")

This plot restates a lot of what we learned in the first plot:  (1) When a candidate has more followers then their lift goes to zero; their following tends to be more independent.  (2) Marianne Williamson has negative lift; her following is not statistically independent of other candidates it is LESS likely to overlap than if we assumed statistical independence.   (3) Bernie Sanders has a big following and his following is relatively independent of other democratic candidates.

I don't think there is much more that is obvious in this data other than the possible link between Sanders and Warren.  Sixty percent of Warren's following follows Sanders, but only 20% of Sanders' following follows Warren.  This is a lot for Sanders.  The log(lift) of the Sanders--Warren link is 0.24.  That is the highest log(lift) for any link between Sanders and the other candidates.   

One purpose of this exercise is to figure out whether people on twitter think the candidates are similar.  I don't really see that in the data.   This twitter dataset tells you that Williamson's followers are not plugged into other candidates (maybe these are from her professional life).  Bernie's following is mostly his own but maybe there is a Sanders--Warren link.  Also the size of a democratic primary candidate's twitter following shapes its the propensity to share followers. 

My best guess as to what shapes the relationship between lift and following:  If an account A is popular then it speaks to a lot of different kinds of people. For account A to have 100% overlap with another account B, all of those different people with different interests will have to take an interest in B.  The bigger the following for account A the less likely that all of its followers will just happen to take interest in the same thing that is not account A.   Just a guess. 

---

The reason that I did this exercise was because the original 538 article's lift plot was a little hard to read. I thought it would work better as a heatmap, but the ordering of the candidates is really important when you visualize it as a heatmap.  It was only when I ranked the candidates by following that the whole thing became clear. 

![alt text](https://github.com/JTS3/538twitteroverlap/blob/master/sharedbytwo_loglift.png "Log(lift) ranked by following")

