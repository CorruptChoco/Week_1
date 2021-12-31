# Overview of Project
The purpose of this Analysis was to provide Louise useful information in a understandable format. To that end I created
2 charts that will be very useful to Louise's goal of creating a successful kickstarter to fund a theater production.

#Analysis Breakdown
##First Chart
The first chart below was created to show the outcomes of theater kickstarters given the month of the year. It was created
by using a pivot table to arrange data such that the sum of outcomes is broken into groups in the columns. Those groups are 
then categorized into rows based on the month of the year. I then used this broken down data to create a line chart to
better visualize the data. Some possible issues with doing this could include putting information in incorrectly within
the pivot table. If the wrong information is added or placed incorrectly you may not get the correct breakdown of information
that you need.
##Second Chart
The second chart below was created to show outcome of kickstarter campaigns in the plays subcategory based on a range of 
goal amounts. The data was curated with the COUNTIFS function within Excel. I used the goal amount, outcome, and subcategory 
of plays to filter the data. In the end and example of the formula used looked like 
`=COUNTIFS(Kickstarter!G:G, "successful",Kickstarter!D:D, "<1,000",Kickstarter!S:S, "plays")` I then used the data we found
to calculate percentage of successful, failed, and canceled. When doing this I did find that if you perform the calculation 
for percentage and include the multiply by 100 in the calculation and then change the format of the cells to percentage you
end up with much higher numbers than anticipated. The solution was to leave the "times 100" out of the calculation.

#Charts
##Chart 1
![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/96025706/147796801-33f3600e-93f3-468c-945f-0c788957d718.png)
##Chart 2
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/96025706/147796813-d394673f-0555-4e0a-b4db-7de83dae75dd.png)

#Questions
##What are two conclusions you can draw about the Theater Outcomes by Launch Date?
From this line chart we can see that for Louise the she is likely to get the best outcome for her kickstarter if her launch date
is between May-Jul. Conversely the worst time to launch would be December as it has the least successful outcomes.
##What can you conclude about the Outcomes based on Goals?
From the line chart we can see that the best outcomes for play kickstarters is when the target goal is between 35000-45000.
##What are some limitations of this dataset?
The limitation of this data is that in some ways it is incomplete. We do not know how much each individual contribution was, we 
can only gain an average. This data does not include information from other crowdfunding sources outside of kickstarter to compare 
our data to. There is also a limited number of data points for more obscure subcategories and is therefore hard to draw conclusions 
on these topics.
##What are some other possible tables and/or graphs that we could create?
Some helpful graphs could include what percent of the whole number of kickstarters are theater kickstarters shown in a pie graph. 
Another could be the breakdown of average donation by category in a pivot table.
