# An Analysis of Kickstarter Campaigns

##Overview of Project

The purpose of this project was to analyze Kickstarter data to uncover trends for successful crowdfunding campaigns, specifically looking at theater and play campaigns.  

##Analysis and Challenges

By formatting the data into a pivot table and filtering the Parent Category to "theater", I was able to compare the successfulness of theater campaigns based on the month they were launched.  The graph below shows how many campaigns were successful, failed or canceled compared to the month that they were launched.  

![Theater Outcomes vs Launch](https://github.com/whitneylosinski/kickstarter-analysis/blob/master/Resources/Theater%20Outcomes%20vs%20Launch.png)

For the next analysis, countif() filters were applied to the data to compare the outcomes of the subcategory "plays" vs the dollar amount of the capmaign goal.  The graph below shows how many successful, failed and canceled play campaigns based on different groups for the dollar amount of the campaign goal.

![Outcomes vs Goals](https://github.com/whitneylosinski/kickstarter-analysis/blob/master/Resources/Outcomes%20vs%20Goals.png)

No challenges/difficulties with the data were found when performing these anlayses but it is important to note that the deadline and launche_at columns of the original data contianed Unix timestamps rather than dates in a standard format.  These columns had to be converted using a timestamp conversion formula of =(((J2/60)/60)/24)+DATE(1970,1,1).

##Results

Looking at the results of the data, it can be determined that theater campaigns are relativley popular and successful campaigns on Kickstarter compared to those in campaigns in other categories.  From the Theater Outcomes vs Launch graph, we can see that May and June appear to be the most successful months to start a theater campaign while November and December appear to be the worst months to start a campaign.

Based on the second graph comparing the outcomes of play campaigns to goal amounts, the data implies that campaigns with pledge goals above $45,000 are not likely to succeed.  Campaigns with goals either less than $1000 or in the $35,000 to $44,999 range tend to have the most success.  


