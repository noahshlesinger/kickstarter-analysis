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



## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
