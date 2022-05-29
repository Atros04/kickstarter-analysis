# Kickstarting with Excel

## Overview of Project

### Purpose
Crowdfunding has been seen as a hit-and-miss system of getting funds for passion projects. *Fever* is one such project where funding was a hit, but how well did we do against other programs that attempted to crowdfund? I wanted to give us an idea of how certain times of the year could affect funding as well as comparing how our funding goal matched to the other plays that have hit Kickstarter.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
Kickstarting plays only started be become popular after 2013; between 2009 and 2013, we saw only 26 campaigns for plays, all of which were successful. From 2014 to 2016, the number of campaigns skyrocketed caping at 518 for the year of 2015 and making this chart finally show failed campaigns. If we omit some of the earlier data and look at 2014-2016 alone, we see that there are fewer successful campaigns to skew our data. 

<img src="https://github.com/Atros04/kickstarter-analysis/blob/main/resources/Theater_Outcomes_vs_Launch_2014_to_2016.png" width=500px> <img src="https://github.com/Atros04/kickstarter-analysis/blob/main/resources/Theater_Outcomes_vs_Launch_2014_to_2016_Overlap.png" width=500px>

Now when we overlap, we can see fewer successful and failed campaigns.

### Analysis of Outcomes Based on Goals
Play goals are even more of a mixed bag as we can see the graph showing no readable trendline. ![The chart shows nothing statistically significant](/resources/Outcomes_vs_Goals.png) Part of this has to do with how few plays were in the funding goals past the $15,000 mark. We counted low twenties after being in triple digits just before that; this low count of plays makes the graph skew and appear to report that successful plays come back at the $35,000-$44,999 marks. Those successful plays were compared against 3 other plays across that range of goal funding.  

### Challenges and Difficulties Encountered
When counting such a large amount of data with really finite filters, we can possibly misrepresent the data. As I was incrimentally changing the `COUNTIFS()` function, I found I had to compare other filtered tables to ensure I was accurately counting and not getting zeroes or other miscounted data. The final step would be the most tricky as defining ranges of data correctly using `<` and `>=` needed to be paired up with their respective rows.

## Results

*- What are two conclusions you can draw about the Outcomes based on Launch Date?*

Time was not really a factor for failed kickstarters. We consistently saw between 30 and 50 failed kickstarters per month among all the data; no one month stood out as a "failure" month over the others. Additionally, we see a larger uptick of successful plays during the spring months meaning that we sould aim to start our campaign in March or April. That being said, there is a slight peak of successful campaigns in the months of October to could serve as a secondary target.

*- What can you conclude about the Outcomes based on Goals?*

Having a goal of $15,000 or lower is ideal, becoming more ideal the less we campaign up to $5,000. 72% of plays that campaigned between $1,000 and $4,999 were successful which is better than the coin flip 55% at $5,000 to $9,999. Additionally, trying to campaign any higher than $25,000 makes our chances catastrophic. 

*- What are some limitations of this dataset?*

This dataset was not able to give us actual donations from backers such as donations that would be considered outliers and we had to rely on averages to give us an idea of how much was donated per backer. And while averages were okay for our current analysis, we could feel pressured about averages during a campaign period. We also are looking at data from 10+ years ago which is not reflective of the trend we see today; kickstarting plays could be much more difficult or easier depending on market saturation.

*- What are some other possible tables and/or graphs that we could create?*

To better represent goal amount, we should use a bar graph whcih can batter give a representation of the histogram trend, skew, and bell vurve (if it exists). The line graph over percentage is nice, but does not do the actual count justice as counts can vary wildly in our raw data from 2 to 515.
Personally, radar charts can give a bit more insight on activity over a time period than line charts do. In that, I would have used a radar to better represent the Outcomes based on launch date.
![Radar Better](/resources/Theater_Outcomes_vs_Launch_Radar.png)
