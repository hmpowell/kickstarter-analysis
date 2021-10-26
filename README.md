# Kickstarting with Excel

## Overview of Project

### Purpose

The purpose of this exercise was to help Louise visualize how successful or unsuccessful different Kickstarters have been based on their launch dates and fundraising goals so she can make an informed decisions about future fundraising projects. In order to showcase this, we analyzed the outcomes of the theater fundraisers based on the month in which they launched, and we analyzed the outcomes of the fundraisers for plays based on the goal amount.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

The analysis of outcomes based on launch date was performed with a pivot table filtered to display only theater fundraisers, with an option to filter for the year. The pivot table had an independent variable of month of initiation of the fundraiser and a dependent variable of the number of outcomes for each of three categories: successful, failed, and canceled. Live kickstarters were not counted in this analysis. The pivot table was then graphed into a line chart to determine which month of launch had the highest number of successful outcomes.

### Analysis of Outcomes Based on Goals

The analysis of outcomes based on goals was performed with a "countifs" function, analyzing information for the subcategory of "plays." Plays was kept constant, while the size of the goal changed, as well as the outcome (i.e. successful, filed, or canceled), were changed to complete the analysis. Once the number of kickstarters were counted for each of the three parameters (plays, goal amount, and outcome of campaign), the percentage of each was calculated based on the total number of projects. This percentage was then graphed in a line chart to determine which size goal had the highest chance of success. Live kickstarters were not counted in this analysis.

### Challenges and Difficulties Encountered

I did not have any challenges in this analysis; however, there were possible difficulties that could arise. In the "Theater Outcomes by Launch Date" pivot table, if the variables were switched, it would be a more difficult to analyze and wouldn't give you the information you wanted. The month should be the independent variable because you'll be able to see which month has the best results. The graph is very condensed when you use the outcome as the independent variable. 

Another challenge could have been found in the "Outcomes Based on Goals" chart. When the "countifs" function is used, there are three or four different criteria that have to be plugged in to the equation, depending on which goal amount needing to be calculated. Entering the wrong column or the wrong goal amount would throw the numbers off, leading to a misunderstanding of the most successful goal to set. 

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

  1. May is the best month, and June is the second best month, to begin a theater Kickstarter, because the chance of success for these months is double the chance of failure.

  2. December is the worst time to start a theater Kickstarter, as the chance of success is almost the same as the chance of failure.

![This is a line graph showing the outcomes based on the launch date of the Kickstarter](https://github.com/hmpowell/kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png)

- What can you conclude about the Outcomes based on Goals?

  - The highest percentage of successful Kickstarters are smaller amounts, less than $1000 or from $1000 to $4999. Initially, as the goals go up, the percentage of success goes down; however, for goals between $35000 and $44999, two-thirds of the outcomes were successful. This would be something into which we should look to determine what other reasons made them successful. Finally, any Kickstarter with a goal above $45000 has a very small likelihood of succeeding. The line graph for this analysis is as follows: 

![This is a line graph showing the outcomes based on the goals of the Kickstarter](https://github.com/hmpowell/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png)


- What are some limitations of this dataset?

  - With each analysis, there is only one independent variable; however, many factors could change why a Kickstarter is successful. The launch date would need to be analyzed by year in addition to the month to see if a certain year had more successful outcomes. The outcomes based on goals are not linear, so it would be interesting to look at why these succeeded or failed, even when the goal was set high. Another independent variable to look into might be the country where the Kickstarters were initiated.

  - The Kickstarters from the "Theater Outcomes by Launch Date" cannot necessarily be compared to the "Outcomes Based on Goals," because the goals are based on plays, while the launch dates are based on all theater fundraisers. The analysis would have to have a consistent category or subcategory to make the two variables more descriptive.

  - The data, in general, does not tell you how the Kickstarter was advertised or how it found donors. This would make a significant difference in how Louise should create a fundraiser. If the person who was initiating a fundraiser had many wealthy friends, the Kickstarter would be more successful faster; whereas, running a Kickstarter without the same affluent contributors would take longer. The data also does not take into consideration which part of the country Louise is located, as the income of the area where she could advertise the most would directly impact how much a contributor might be able to give. In a wealthier area of the country, a contributor might be able to give more than a low-income location. 

- What are some other possible tables and/or graphs that we could create?

  - A few ideas for graphs are as follows:

    1. A line graph with the independent variable as month and year of launch and the dependent variable as the outcome would give us a longer look at how the Kickstarter outcomes ebb and flow and might give us a look into whether the more successful months are in the same year or different years.

    2. To dive deeper into the plays in the US that Louise is interested in learning more about, a line graph from a pivot table filtered by country and month could be used, and rather than the number of outcomes of theater fundraisers, it would be the number of play fundraisers in particular.

    3. To find out if the success of a fundraiser came from larger donors, we could create a line graph with the independent variable of average donation (broken down into different increments) and the dependent variable of outcomes. The higher the average donation, the wealthier the contributors; this might give us a look into how many donors Louise might need to succeed in her fundraiser, depending on what she anticipates as the average donation from people she may know or the area in which she lives.
