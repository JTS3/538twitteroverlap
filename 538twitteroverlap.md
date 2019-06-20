# A Brief Note on 538 Twitter Overlap


In the data gathered for this [data journalism piece](https://fivethirtyeight.com/features/which-2020-candidates-have-the-most-in-common-on-twitter/) by Gus Wezerek [@guswez](https://twitter.com/guswez) or and Oliver Roeder [@ollie](https://twitter.com/ollie),  lift is a function of the number of followers. 

The larger a candidate's twitter following the more isolated that following tends to be. 538 present the data as a table which as a default is sorted by exclusive followers.  You should really compare the two. 

The Williamson following's isolation stands out relative to her following's size; her name is high above the OLS line.  To a lesser extent we see the same kind of isolation happening with Hickenlooper, Yang, and Gabbard.  Wezerek and Roeder note Warren's followers gregariousness; they are far below the OLS line.  A similar thing could be said of Swalwell, did you know that 72% of Swalwell fans also follow Harris?

![alt text](https://github.com/JTS3/asides/blob/master/sharedbytwo_exclusivefollowers_followers.png "Exclusive Followers v Followers")

Wezerek and Roeder use lift to get at the independence of following one candidate or the other.  Below I plot log(lift) against log(followers). When log(lift) is zero, then lift is one and the events are independent.  When log(lift) is below zero, then sharing a follower is less likely than if you assumed following was independent. 

![alt text](https://github.com/JTS3/asides/blob/master/sharedbytwo_loglift_logfollowers.png "Lift v Followers)

This plot restates a lot of what we learned in the first plot:  (1) When a candidate has more followers then their lift goes to zero; their following tends to be more independent.  (2) Marianne Williamson has negative lift; her following is not statistically independent of other candidates it is LESS likely to overlap than if we assumed statistical independence.   (3) Bernie Sanders has a big following and his following is relatively independent of other democratic candidates.

I don't think there is much more that is obvious in this data other than the possible link between Sanders and Warren.  Sixty percent of Warren's following follows Sanders, but only 20% of Sanders' following follows Warren.  This is a lot for Sanders.  The log(lift) of the Sanders--Warren link is 0.24.  That is the highest log(lift) for any link between Sanders and the other candidates. 

One purpose of this exercise is to figure out how people on twitter think about the candidates.  This twitter dataset tells you that Williamson's followers were not plugged into other candidates (maybe these are from her professional life), and Bernie is to a lesser exent his own but maybe there Sanders--Warren link.  Also the size of a candidate's twitter following seems to determine the propensity to share followers. 
