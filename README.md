### Utopia Tableau Dashboard Link: 
[Tableau Dashboard](https://public.tableau.com/views/UtopiaFinalProject/MainPage?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)



### Table of Contents
#### [Tableau Dashboard](#Utopia)
#### [Motivation](#Motivation)
#### [Questions](#Questions)
#### [Normalizing the Data](#Normalizing_the_Data)
#### [Categorization & Calculation Process](#Categorization_&_Calculation_Process)
#### [Challenges](#Challenges)
#### [Technologies Used](#technologies-used)
#### [Sources](#Sources)
#### [Conclusion](#Conclusion)




#### Motivation
Growing up in the United States, I was often led to believe that the United States was one of the best nations in the world.  I believe public schooling often teaches American children to focus on the positives of the United States, without fully acknowledging the shortcomings of our country or the ways in which other nations surpass us.  I wanted to illustrate the different strengths and weaknesses of major countries all over the world, while highlighting potential interesting correlations and giving a numeric weighted score to each country, based on physiological, psychological, and emotional needs and how those needs are addressed by each governing body.


#### Questions

Which countries fail to meet its citizens basic needs, and what countries best meet them?
Which countries rank as the safest and most unsafe in comparison to one another?
Is there a correlation between reported happiness levels and longer levels of schooling? What about happiness and access to the internet?

#### Normalizing the Data

To ensure that all features contributed equally to the analysis, I normalized the dataset prior to modeling. Normalization helped to bring all numeric variables onto a comparable scale. I came across a formula online that worked well for this:

dataframe['normalized_column'] = (dataframe['column']   - dataframe['column'].min()) / (dataframe['column'].max() - dataframe['column'].min())

--
This formula ensure that every value was converted to value of anywhere from 0 to 1. Because I wanted my point system to reflect a higher number of points being more preferable, I had to adjust my formula in instances where the original data reflected a higher score as being less favorable. To do this, I simply adjusted the formula by adding a "1-" at the beginning of the formula. Here's how that looked:

dataframe['normalized_column'] = (dataframe['column']   - dataframe['column'].min()) / (dataframe['column'].max() - dataframe['column'].min())

#### Categorization & Calculation Process

Once my data was normalized, I then multiplied each value by it's corresponding weight based on a descending logarithmic scale, starting at 32. To determine the weight in which each value was to be multiplied, I categorized each metric into one of four categories: A, B, C, & D. I based this categorization system off of the psychological concept known as "Maslow's Hierarchy of Needs": 

Category A: Basic Needs, weight of 32
Category B: Safety & Security, weight of 16
Category C: Education, Family, & Relationships, weight of 8
Category D: Collective Responsiblity, Achievement, & Happiness, weight of 4

So, for example, if a country scored a perfect 1 in a metric in category A, that metric would give the country 32 points.  If this same score occured in category B, the country would be awarded 16 points, and so on.


#### Challenges

Despite a lot of these metrics being obtained by the same organizations, many of them did not have universalized country names. For example, The United Kingdom sometimes showed up as Great Britain, or the UK.  To combat this, I installed and imported "country_converter". This didn't fix all the issues, but it did limit how many countries I was inadvertently losing due to attempting to merge data frames with non-matching names.

The datasets I was able to obtain did not have a large number of overlapping years. That said, I did my best to filter each dataset down to the most recent years with sufficient measurements. All datasets come from a ten year period of time (2015 - 2025).


#### Technologies Used

Python / Pandas - for exploration, normalizing and aggregation of the dataset
Tableau - for creating interactive dashboard
Figma - for introduction of Project
Canva - for introduction of Project
Git - for version control

#### Data Sources
To answer the above questions I used the following sources to collect datasets for my analysis:
-[Basic Water](https://ourworldindata.org/grapher/population-using-at-least-basic-drinking-water)
-[Basic Sanitation](https://ourworldindata.org/grapher/share-using-safely-managed-sanitation)
-[Life Expectancy](https://ourworldindata.org/grapher/life-expectancy-hmd-unwpp?tab=table)
-[Pollution](https://ourworldindata.org/grapher/pm25-air-pollution)
-[Insufficient Calories](https://ourworldindata.org/grapher/number-calorie-diet-unaffordable)
-[Unemployment](https://ourworldindata.org/grapher/unemployment-rate)
-[Terrorist Attacks](https://ourworldindata.org/grapher/terrorist-attacks)
-[Functioning Government Index](https://ourworldindata.org/grapher/functioning-government-index-eiu)
-[Crime Rate](https://worldpopulationreview.com/country-rankings/crime-rate-by-country)
-[Universal Healthcare Index](https://ourworldindata.org/grapher/universal-health-coverage-index)
-[Atkinson Inequality Index](https://ourworldindata.org/grapher/income-inequality-atkinson-index-undp)
-[Equal Rights Protection Index](https://ourworldindata.org/grapher/equal-rights-protection-index)
-[Years of Schooling](https://ourworldindata.org/grapher/mean-years-of-schooling-long-run)
-[Depression Rates](https://ourworldindata.org/grapher/depressive-disorders-prevalence-ihme)
-[LGBT+ Equality Index](https://ourworldindata.org/grapher/lgbt-legal-equality-index)
-[Suicides per 100k](https://ourworldindata.org/suicide)
-[Research Articles Published Yearly](https://ourworldindata.org/grapher/scientific-publications-per-million)
-[Happiness Index](https://ourworldindata.org/grapher/happiness-cantril-ladder)
-[Freedom of Expression](https://ourworldindata.org/grapher/freedom-of-expression-index)
-[Human Development Index](https://ourworldindata.org/grapher/human-development-index)
-[Percent of Renewable Energy](https://ourworldindata.org/grapher/share-electricity-renewables)

#### Conclusion

The list of top countries by my scoring system was dominated heavily by Europe, specifically Scandanavia and other Northern European countries.  Iceland, Norway, and Denmark each appeared in all of the top 15 lists. No countries consistently appeared in all of the bottom 15 lists, however Ethiopia did appear in A,B,C, and the "All Categories" bottom 15 list. Only 1 country appeared in the top 30 of a category while appearing in the bottom 30 of two other categories, and that was the United Arab Emirates.  UAE scored in the top 30 for category B, but in the bottom 30 for categories C and D.



About
No description, website, or topics provided.
Resources
 Readme
 Activity
Stars
 0 stars
Watchers
 1 watching
Forks
 0 forks
Report repository
Releases
No releases published
Packages
No packages published
Languages
Jupyter Notebook
100.0%
Footer
©