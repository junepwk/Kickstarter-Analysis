# Kickstarting with Excel

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#overview-of-project">Overview of Project</a>
      <ul>
        <li><a href="#purpose">Purpose</a></li>
      </ul>
    </li>
    <li>
      <a href="#analysis-and-challenges">Analysis and Challenges</a>
      <ul>
        <li><a href="#analysis-of-outcomes-based-on-launch-date">Analysis of Outcomes Based on Launch Date</a></li>
        <li><a href="#analysis-of-outcomes-based-on-goals">Analysis of Outcomes Based on Goals</a></li>
        <li><a href="#challenges-and-difficulties-encountered">Challenges and Difficulties Encountered</a></li>
      </ul>
    </li>
    <li><a href="#results">Results</a></li>
  </ol>
</details>

## Overview of Project

### Purpose

The main purpose of this analysis was to help Louise, a playwright, uncover any trends and patterns to a successful Kickstarter campaign. Louise estimated that her play expenses would exceed $10,000 and she would like to know what are some factors to consider to ensure that her crowdfunding campaign would meet her goal. The factors that were focused on in this analysis were funding goals set for campaigns, launched dates of the campaigns and their correlation with the overall campaign's outcome (successful, failed, or canceled).

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

In this analysis, outcomes of campaigns for the theater category were perused based on their launched date by creating a pivot table of the dataset, filtering 'Parent Category' to theater and 'Years' of each campaign launched.  With a total of 111 successful and 52 failed campaigns out of a total of 166 projects, May is the month in which the most kickstarter campaigns accomplished their goal.  This is closely followed by June with 100 'successful' and 49 'failed' out of 153 projects.  Additionally, May, June, July and 
October all have approximately the same number of failed projects.  

![Theater_Outcomes_vs_Launch](https://github.com/junepwk/kickstarter-analysis/blob/main/resources/Theater_Outcomes_vs_Launch.png)

This analysis shows that May is the prime month to kickstart a theater crowdfunding event, but Louise's plan is specifically for a play. In the next section, there will 
be a deeper dive to uncover additional factor(s) that might contribute to the success rate of theater play campaigns by comparing their outcomes based on goals.

### Analysis of Outcomes Based on Goals

By narrowing the focus down to subcategory 'plays', it is evident that the dollar amount range for goals with the highest success rate are set between 'less than 1000' and 
'1000 to 4999'.  In the range, 'less than 1000', there is a 76% success and 24% fail rate out of a total of 186 projects.  In '1000 to 4999', there is a 73% success 
and 27% fail out of a total of 534 projects.  The next runnerup ranges are set between '35000 to 39999' and '40000 to 44999' with 67% success and 33% fail for both.  These goals are set quite high and there are only a total of 6 projects and 3 projects, respectively.  Therefore, there might be other factors that played a part in their
achievements.  This piece of information could be a concern for Louise as her goal is greater than $10,000.  Within her range, '10000 to 14999', there is a 54% success
and 46% fail rate out of a total of 72 projects.  Although, in the 'plays' subcategory, there appears to be no 'canceled' campaigns, Louise's plan for her Kickstarter crowdfunding event could have a close possibility of either failing or succeeding. 

![Outcomes_vs_Goals](https://github.com/junepwk/kickstarter-analysis/blob/main/resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered

In the first analysis, the pivot table had created a separate subcategory named "(blank)" for both the "Parent Category" and "Column Labels" after I had arranged the variables
into their fields.  However, since I'll be filtering the table for just 'theater', 'successful', 'failed' and 'canceled', it was not a major concern.  The second analysis 
is where I encountered more difficulties.  Aside from the usual misspelling of words in the formula or misplaced syntax, I found creating the dollar amount ranges in the formula
to be challenging.  After trial and error and surveying the example video provided, I was able to create the range with the correct syntax.  Lastly, the final table created felt a little clustered with numbers so using conditional formatting in Excel, I did color scaling for the columns "Percentage Successful" and "Percentage Failed" so that it is visually easier to identify any patterns. 

## Results

- Conclusions based on Launch Date:

First, May is prime time for Louise to launch her future campaign(s) in the theater category with the month of June being a close second. Secondly, December is a terrible month
for theater related campaigns as there appears to be a 50/50 chance for success and fail. If Louise was to launch her campaign for her play "Fever", I would highly suggest doing so in the 
month of May.  

- Conclusion based on Goals:

Campaigns with goals that are less than or equal to $4,999 have the highest chance of success, which makes sense considering it'll take less money donation to achieve their goal.  In Louise's case, with a budget of over $10,000, based on the Kickstarter dataset, her campaign would have a 54% chance of succeeding and 46% chance of failing. I would suggest a thorough review of her budget itinery to cut out some expenses if she would like a higher chance of her campaign being successful. 

- Limitations of this dataset:

In the first analysis, it was filtered to show 'theater' campaigns' outcomes.  Within this category, there are a total of three subcategories named 'plays', 'musical', and 'spaces'. This means that the data gathered could be too vague to make an accurate conclusion for the client Louise as she is interested in launching a campaign for a play.  Although, it was concluded that May is a great time to launch theater campaigns, it is unclear rather it is still an accurate representation for play projects. 

The second analysis, by filtering the data to 'plays', provided a more indepth and relatable data for Louise.  However, the number of projects with goals above $15,000 are significantly lower than the number of projects with goals less than $15,000. Therefore, the outcome ratio for projects with goals above $15,000 might not have an accurate representation since the sample size is so small.   

- Other possible tables and/or graphs that could be utilized:

We could create a pivot table that filtered the parent category, years, and the subcategory. For the second analysis, we could consider adding columns for "Average Donation" because the trend seems to follow that the lower the goal is set the higher the success rate.  But you could see that the ranges '35000 to 39999' and '40000 to 44999' both have the third highest success rate.  By including "Average Donation", we could see whether it was due to a high number of donations.  
