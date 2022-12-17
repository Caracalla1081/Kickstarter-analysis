# Kickstarting with Excel

## Overview of Project
Having already provided Louise with analysis that aided her in choosing her fundraising goal, she was curious to see how different campaigns performed in relation to their launch datas and funding goals.
### Purpose
The pruprose of this analysis is to provide Louis with data to give her insight into whether there are any correlations to be drawn between a kickstarter campaign's start month and its goal. 
## Analysis and Challenges
Working with raw data for kickstarter campaigns from May 2009 to March 2017; the data first needed to be formatted in order to create visuals based on measurements of date/time.
- First, by utilizing the "date created conversion" column and the YEAR() function, I was able to extract just the year from the "date created conversion" timestamps. This allowed me then to create a pivot table, and ultimately a pivot chart titled "Theater Outcomes Based on Launch Date"; displaying the counts of kickstarter campaigns where the outcomes were either "successful", "failed", or "canceled", by month.
- Second, I utilized the COUNTIFS() function to create a table that not only broke down the counts of campaigns that fell into "successful", "failed", or "canceled"; but also sorted by conditions based on various ranges of goals (0-999, 1000-4999, etc.) and by the subcategory "plays". The chart was then extended to include percentages of each category of kickstarter campaign outcome by dividing their counts of each outcome vs. goal range by the total of campaign outcome counts.
As a result I then created a line graph showing the relationship between a kickstarter campaigns outcome vs. its goal range.
### Analysis of Outcomes Based on Launch Date
![Alt text](../../../../../OneDrive/Desktop/Data%20Bootcamp%20Class%20Folder/Module%201/Challenge/Resources/Theater_Outcomes_vs_Launch.png)
Utilizing the aforementioned pivot chart titled "Theater Outcomes Based on Launch Date", the analysis leads to the conclusion that "theater" kickstarter campaigns started in May appear to have the most amount of success, followed by June and July to round out the top three. Whereas this may tell us the count of outcomes based on starter month, it does not give us enough detail in breaking down where the "successful", "failed", or "canceled" outcome counts would land if we included the goal amounts. Thus, we need to dig deeper into the actual goals of these outcome categories.
### Analysis of Outcomes Based on Goals
![Alt text](../../../../../OneDrive/Desktop/Data%20Bootcamp%20Class%20Folder/Module%201/Challenge/Resources/Outcomes_vs_Goals.png)
Looking at the "Outcomes Based on Goal" chart, I was able to gain better insight into exaclty how a kickstarter campaign's goal impacts its outcome. Keeping the "plays" kickstarter campaign goal between the range of $1 to $4,999 puts the chance of success at 73%, greater than the overall succes rate of 66%. Generally speaking as the goal amount for the kickstarter campaign rises, the "success" rate drops and the "failed" rate rises. There is a point in which the lines for "success" and "failed" cross paths again to reverse this trend, but with only nine total campaigns between this goal range of $35,000 and $44,999 there is not a big enough sample size there for me to recommend that risk is worth the reward if truly not needed.
### Challenges and Difficulties Encountered
The main challenge that I faced was in my COUNTIFS() function. I gave it a go several times unassisted, but I am still making mistakes with proper punctuation in my formulas; so I watched the "hint" video. to successfuly write the formula.
Another mistake I made was user error where I had the wrong column identified in my formula for "outcome", and only after about 30mins of checking and testing my formula;ultimately copying the formula in the rest of the "Outcomes Based on Goals' table, did I realize the mistake and corrected it.
## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
"Theater" kickstarter campaigns started in May appear to have the most amount of success, followed by June and July to round out the top three. 
Also by utilizing what can be inferred by the months in relation to campaign launches and the solid assumptions of people's spending habits; May seems to hit the sweetspot of people just getting through any bills related to winter holiday spending, but before summer vacations hit. Potentially increasing peoples disposable income, and willingness to donate.
- What can you conclude about the Outcomes based on Goals?
A "plays" kickstarter campaign's success can be confidently tied to the amount of the goal. Most organizers of campaigns seem to be aware of this, thus the higher count of campaigns at the lower level of goal amount as opposed to the higher levels. Also, there seems to be a bit of success between the $35,000 to $44,999 goal range, but any higher leads to failure.
- What are some limitations of this dataset?
Some limitations in this dataset to me are I would like to know the economic makeup of the donors. This could give more insight into potentially why a few of the higher goal range kickertarter campaings were successful. Also, the makeup of these plays; cast, set pieces, crew, etc. If there is a description of the size and details of the play provided might that lend to more giving with potential donors feeling it is justified. 

- What are some other possible tables and/or graphs that we could create?
One other table/graph I would like to have seen created is an "Outcome Based on Length of Campaign". This could potentially answer why the few higher goal kickstarter campaings were successful over others.
I would also have liked to see some of the created charts drilled down by country, or even origin of donations. That would be interesting to see if there is just more interest in certain kickstarter campaigns, or willingess for people to donate based on the region the kickstarter is based in or where the donations originate from.