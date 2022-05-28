# Kickstarting with Excel

## Overview of Project

### Purpose
Crowdfunding has been seen as a hit-and-miss system of getting funds for passion projects. *Fever* is one such project where funding was a hit, but how well did we do against other programs that attempted to crowdfund? I wanted to give us an idea of how certain times of the year could affect funding as well as comparing how our funding goal matched to the other plays that have hit Kickstarter.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
Time was not really a factor for failed kickstarters. We consistently saw between 30 and 50 failed kickstarters per month among all the data; no one month stood out as a "failure" month over the others. However, we do see a larger uptick of successful plays during the spring months. ![Nothing to see here](/resources/Theater_Outcomes_vs_Launch.png) That being said, there is a slight peak of successful campaigns in the months of October over the negative trend we see starting from May.

### Analysis of Outcomes Based on Goals
Play goals are even more of a mixed bag as we can see the graph showing no readable trendline. ![The chart shows nothing statistically significant](/resources/Outcomes_vs_Goals.png) Part of this has to do with how few plays were in the funding goals past the $15,000 mark. We counted low twenties after being in triple digits just before that; this low count of plays makes the graph skew and appear to report that successful plays come back at the $35,000-$44,999 marks. Those successful plays were compared against 3 other plays across that range of goal funding.  

### Challenges and Difficulties Encountered
When counting such a large amount of data with really finite filters, we can possibly misrepresent the data. As I was incrimentally changing the `COUNTIFS()` function, I found I had to compare other filtered tables to ensure I was accurately counting and not getting zeroes or other miscounted data. The final step would be the most tricky as defining ranges of data correctly using `<` and `>=` needed to be paired up with their respective rows.

## Results

*- What are two conclusions you can draw about the Outcomes based on Launch Date?*
Franky, not much. Kickstarting plays only started be become popular after 2013; between 2009 and 2013, we saw only 26 campaigns for plays, all of which were successful. From 2014 to 2016, the number of campaigns skyrocketed caping at 518 for the year of 2015 and making this chart finally show failed campaigns. If we omit some of the earlier data and look at 2014-2016 alone, we see that there are fewer successful campaigns to misrepresent the times. ![Sectional Chart](/resources/Theater_Outcomes_vs_Launch_2014_to_2016.png) What we then find when we overlap this chart with our original is a more relaistic picture. ![overlap chart](/resources/Theater_Outcomes_vs_Launch_2014_to_2016_Overlap.png)

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
