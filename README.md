# Excel-challenge
Organize and analyze a database of 4,000 past projects in order to uncover any hidden trends

In this project I will be using the Excel table provided, modify and analyze the data of 4,000 past Kickstarter projects as I attempt to uncover some market trends.


- I used conditional formatting to fill each cell in the state column with a different color, depending on whether the associated campaign was successful, failed, or canceled, or is currently live.
  - I created a new column 'O' called `Percent Funded` that uses a formula to uncover how much money a campaign made to reach its initial goal.
  
- I used a conditional formatting to fill each cell in the `Percent Funded` column using a three-color scale. The scale should start at 0 and be a dark shade of red, transitioning to green at 100, and blue at 200.
  - I created a new column 'P' called `Average Donation` that uses a formula to uncover how much each backer for the project paid on average.
  - I created two new columns, one called Category at Q and another called Sub-Category at R, which use formulas to split the Category and Sub-Category column into two parts.
  - I created a new sheet with a pivot table that will analyze my initial worksheet to count how many campaigns were successful, failed, canceled, or are currently live per **category**.
  - I created a stacked column pivot chart that can be filtered by country based on the table you have created.
  - I created a new sheet with a pivot table that will analyze the initial sheet to count how many campaigns were successful, failed, or canceled, or are currently live per sub-category.
  - I created a stacked column pivot chart that can be filtered by country and parent-category based on the table you have created.

- The dates were stored within the deadline and launched_at columns use Unix timestamps. 
  - A new column named Date Created Conversion was created that will use this formula to convert the data contained within launched_at into Excel's date format.
  - I created a new column named `Date Ended Conversion` that will use [this formula](https://www.extendoffice.com/documents/excel/2473-excel-timestamp-to-date.html) to convert the data contained within deadline into Excel's date format.
- I created a new sheet with a pivot table with a column of `state`, rows of `Date Created Conversion`, values based on the count of `state`, and filters based on `parent category` and `Years`.


##  Observations
From the visulaizations, a report which answered the following questions could me made
1. What are three conclusions we can draw about Kickstarter campaigns?
2. What are some limitations of this dataset?
3. What are some other possible tables and/or graphs that we could create?



###                                       Saheed Obitayo
###                                     Kick Start My Chart
1) From the Data provided, we can conclude that most kick starter campaigns originate from the United States of America as that is the country with the most projects. Additionally, we can conclude that most of the Kickstarter campaigns are plays. Lastly, we can conclude that if successful campaign should be created, the best move would be for it to fall into a rock category as that has proven to be the most successful campaigns with a 100% success rate based on the data. 

2) **Lack of Previous Data**: The main limitation of this dataset is that there is no representation with the populations of the dataset. The most recent 4,000 campaigns were analyzed out of 300,000 campaigns. The sample size of about 1.3% is not big enough to show the true trends of Kickstarter campaigns especially when there’s no method for data collection and just shows the most recent campaigns. External factors happening in the world could have affected the success of each campaign that was not accounted for. It would be better is the data was spread across multiple dates instead of just the most recent date.

3) **Pie Chart**: Show the percentage of a value as each slice represents a different category. We can see how each subcategory looks compared to the other subcategories.  
**Bar chart**: This can be used to show a distribution of data points and comparison across different groups. We can see which groups have the most and least in common as well as lowest and highest values.

#### BONUS
1)	Based on the data, the median summarizes the data more meaningfully. This was observed from the boxplots of the unsuccessful and successful backer count values.
2)	Based on the data, there is a greater variability in backer count in successful campaigns than unsuccessful ones. This makes sense because although successful campaigns typically require greater number of backers, it can also have a smaller backer count if the average donation is higher. Unsuccessful campaigns will always have a smaller backer count as a larger backer count would turn the unsuccessful campaign successful.






Bonus


Create a new sheet with 8 columns:

Goal
Number Successful
Number Failed
Number Canceled
Total Projects
Percentage Successful
Percentage Failed
Percentage Canceled



In the Goal column, create 12 rows with the following headers:

Less than 1000
1000 to 4999
5000 to 9999
10000 to 14999
15000 to 19999
20000 to 24999
25000 to 29999
30000 to 34999
35000 to 39999
40000 to 44999
45000 to 49999
Greater than or equal to 50000




Using the COUNTIFS() formula, count how many successful, failed, and canceled projects were created with goals within the ranges listed above. Populate the Number Successful, Number Failed, and Number Canceled columns with this data.


Add up each of the values in the Number Successful, Number Failed, and Number Canceled columns to populate the Total Projects column. Then, using a mathematical formula, find the percentage of projects that were successful, failed, or canceled per goal range.


Create a line chart that graphs the relationship between a goal's amount and its chances at success, failure, or cancellation.



Bonus Statistical Analysis
If one were to describe a successful crowdfunding campaign, most people would use the number of campaign backers as a metric of success. One of the most efficient ways that data scientists characterize a quantitative metric, such as the number of campaign backers, is by creating a summary statistics table.
For those looking for an additional challenge, you will evaluate the number of backers of successful and unsuccessful campaigns by creating your own summary statistics table.


Create a new worksheet in your workbook, and create a column each for the number of backers of successful campaigns and unsuccessful campaigns.



Use Excel to evaluate the following for successful campaigns, and then for unsuccessful campaigns:


The mean number of backers.


The median number of backers.


The minimum number of backers.


The maximum number of backers.


The variance of the number of backers.


The standard deviation of the number of backers.




Use your data to determine whether the mean or the median summarizes the data more meaningfully.


Use your data to determine if there is more variability with successful or unsuccessful campaigns. Does this make sense? Why or why not?
