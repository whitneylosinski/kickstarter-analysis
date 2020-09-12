# An Analysis of Kickstarter Campaigns

##Overview of Project

The purpose of this project was to analyze Kickstarter data to uncover trends for successful crowdfunding campaigns, specifically looking at theater and play campaigns.  

##Analysis and Challenges

By formatting the data into a pivot table and filtering the Parent Category to "theater", I was able to compare the successfulness of theater campaigns based on the month they were launched.  The graph below shows how many campaigns were successful, failed or canceled compared to the month that they were launched.  

![Theater Outcomes vs Launch](https://github.com/whitneylosinski/kickstarter-analysis/blob/master/Resources/Theater%20Outcomes%20vs%20Launch.png)

For the next analysis, countif() filters were applied to the data to compare the outcomes of the subcategory "plays" versus the dollar amount of the capmaign goal.  The graph below shows the percentage of successful, failed and canceled play campaigns based on the dollar amount of the campaign goal.

![Outcomes vs Goals](https://github.com/whitneylosinski/kickstarter-analysis/blob/master/Resources/Outcomes%20vs%20Goals.png)

No challenges/difficulties with the data were found when performing these anlayses but it is important to note that the deadline and launched_at columns of the original data contained Unix timestamps rather than dates in a standard format.  These columns had to be converted using a timestamp conversion formula of =(((J2/60)/60)/24)+DATE(1970,1,1).

##Results

- Looking at the results of the data, it can be determined that theater campaigns are relativley popular and successful campaigns on Kickstarter compared to campaigns in other categories.  From the Theater Outcomes vs Launch graph, we can see that May and June appear to be the most successful months to start a theater campaign while November and December appear to be the worst months to start a campaign.

- Based on the second graph comparing the outcomes of play campaigns to goal amounts, the data implies that campaigns with pledge goals above $45,000 are not likely to succeed with a success rate of less than 20%.  Campaigns with goals either less than $4999 or in the $35,000 to $44,999 range tend to have the most success.  

- There are some limitations to this data set that should be considered.  For example, it is not clear what determines if a campaign is "Successful".  Does successful mean that the campaign reached it's monetary goal or does it mean that the project was carried out to completion and on time?  Another thing to consider is that this data set only contained data for 4,109 campaigns but the Kickstarter website states that it has over 185,000 successful campaigns.  This implies that the data set used is only a sample of all the Kickstarter projects and it is not clear how this sample was chosenor if it effectively represents all Kickstarter campaigns.

- To dive further into this data and uncover additional trends, it may be useful to compare the level of success based on location or the length of the campaign.  Another thing to consider is the amount of success versus the number or backers or the average donation.  These insights may uncover trends in the campaign data that could be useful for determining the best chance for launching a successful campaign.
