# An Anaylis of Kickstarter Campaigns
## Louise has a play she wants to get funded through a kickstarter campaign with an estimated monetary requirement 4000 euros and needs to understand what makes a campaign successful. 

### The purpose of this document is to outline pertinent trends in previous kickstarter campaigns to aid Louise in meeting her funding goal. 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
The first important question to answer is *when* Louise should initiate her kickstarter campaign. The following chart demonstrates not only when kickstarters are typically started throughout the months of the year but also includes whether or not it was successful, a failure, or canceled before completion. To make this more relevant to Louise's particular interest in theater related campaigns, the data has been filtered to only include those such campaigns. 

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/95305584/147966870-fd9f8f7a-681a-4067-adf9-24ef5d03eb2f.png)

All the data used in this report is taken from a spreadhsheet (
[Kickstarter_Challenge.xlsx](https://github.com/noahshlesinger/kickstarter-analysis/files/7803645/Kickstarter_Challenge.xlsx))  containing over 4000 kickstarter campaigns with varoius data points such as date of launch, funding goal, pledged amount, outcomes, etc. The first step in creating the above diagram was creating a pivot table in a new worksheet containing all the data from the original worksheet. The next step involved appropriately assigning the data of interest (here the launch date and outcomes) in the pivot table fields to create the pivot table which would be filtered for theater campaigns. Last step was to plotting the outcomes as a function of time acros 12 months. The pivot table can be viewed in the excel workbook under the "Theater Outcomes by Launch Date" worksheet tab.

As is evident, the number of canceled campaings is relaitively low throughout the year while failed and successful campaigns show an increase in the summer months. By looking at the failed and successful campaigns together, it becomes clear that the most popular time of to start a campaign is in those summer months, specifically in June. 

### Analysis of Outcomes Based on Goals
Another important factor to consider when Louise is creating her campaign is whether or not her funding goal is reasonable. The chart below represents the number of successful and failed campaigns categorized into funding goal in increments of roughly $5,000 starting at $1,000. Again, having data on all campaigns could lead to a inaccurate conclusion given Louise's specific focus on plays, and, therfore, the graphs represents only kickstarters campaigning for play. 

![Outcomes_vs_Goals png](https://user-images.githubusercontent.com/95305584/147966731-bb817eed-c4ff-437c-a9dc-366f1d304241.png)

Similar to the previous plot, the data used here was taken from the "Kickstarter_Challenge" data set.  In order to create the percentages for outcomes as a funciton of goal amount, the functions "VLOOKUP()" and "SUM()" were used to gather the relevant data. Once the number of successful, failed, and canceled campaigns was filled out in correlation with the goal amounts, they were summed to create a total, then taken over the sum to create percentages for each outcome. 

The graph shows no canceled campaigns in the above ranges, indicating that all campaigns for plays were either successful or failed. It also shows an inverse relationship between successful campaigns and goal amounts. This is opposite to the relationship between failed campaigns for plays and the goal amount.
### Challenges and Difficulties Encountered

In dealing the with excel, the most common error I made was incorrectly typing a formula. Calling data from different sheets was initally challenging as was using novel formulas. In creating the graph "outcomes based on goal", it took some time to learn the different ways of typing information into the formula depending on what type of text it was going to be using. switching between general text, to accounting, to looking at a cell as whole took some getting used to. Lastly, not knowing why something was amiss or not working was perhaps the most challenging as not knowing where to begin looking and making sure not to overlook certain parts was difficult. 

## Results

- From the Outcomes based on the Launch Date, it is clear that, for Louise, the optimal time to start her campaign is in the months of may and june as those show the greatest number of successful campaigns. If you look at it as a ratio, the moth of may has the greatest success to failure with June in second. The opposite is true in the fall and early winter months in which the successful campaigns don't outnumber the failed ones by as much. One thoughtprocess for why this is could be that in the last several months of the fiscal year, companies and potential donors may be thinking about their financial numbers and be less ready to give to a kickstarter campaign. Looking back to the summer months, there is a general understanding that with the sun out and warm weather everpresent, leisure activities such as going to a theater or play sounds more enticing and investing/supporting one might be easier to do for some. 

- Luckily for Louise, she is in one of the better ranges given her goal of 4,000 euros (~$5,000). With the downward trend for sucessful campaigns vs goal amounts, she wouldn't want to consider increasing her goal any further. It is worth noting that there is a sudden uptick in successful campaigns in the $35,000-$45,000 range. My only speculation is that there are different levels of plays: smaller and more local plays that don't require much in terms of production, and large broadway type productions that require more logistical and ellaborate planning. 

- With this data set, we aren't able to determine how the data points were collected. There is a difference between volunteering up information and collecting it from kickstarter's website. For example, it could skew the data to show more successful campaigns given that failed campaigns may be less willing to share their failure with the public. Another, yet small detail missing, is current information. There aren't any campaigns in the workbook after 2017 and with the modern era demonstrating that trends in popularity of the general population can change year to year drastically, it would be helpful to have more up-to-date information. Furthuremore, there is no real way to determine why a given campaign failed or succeeded. If there was description of the cause for success and failure, it would be more beneficial for Louise. In this report, there are only trends, correlations, but no causations. There can only be specualtion that if she has a low goal and launches her campaign in May or June that it will be successful but only based off of trends. The data also doesn't show how the kickstarter campaigns were marketed, which could have a significant impact on overall success. 

- Other graphs to include could be:
  * Outomces as a funciton of year to see whether there is a trend at all over time indicating increase/decrease in successful campaigns.
  * An additional graph to compliment the Outcomes Based on Launch Date section that focused in on the month of May and June to determine of there is a sweetspot to launch. 
  * Lastly, an additional column could be created to better categorize the plays into genres, and then plot outcomes based as a function of genres. To go a step further would be to determine if certain genres were more successful at different types of the year. 
