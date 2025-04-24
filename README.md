Utopia
Tableau Dashboard
Link: 
[Tableau Dashboard](https://public.tableau.com/views/UtopiaFinalProject/MainPage?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)



# Table of Contents
## Tableau Dashboard
## [Motivation](#Motivation)
## Questions
## Normalizing the Data
## Challenges
## Technologies Used
## Sources
## Conclusion




### Motivation
Growing up in the United States, I was often led to believe that the United States was one of the best nations in the world.  I believe public schooling often teaches American children to focus on the positives of the United States, without fully acknowledging the shortcomings of our country or the ways in which other nations surpass us.  I wanted to illustrate the different strengths and weaknesses of major countries all over the world, while highlighting potential interesting correlations and giving a numeric weighted score to each country, based on physiological, psychological, and emotional needs and how those needs are addressed by each governing body.


### Questions

Which countries fail to meet its citizens basic needs, and what countries best meet them?
Which countries rank as the safest and most unsafe in comparison to one another?
Is there a correlation between reported happiness levels and longer levels of schooling? What about happiness and access to the internet?


Challenges

Despite a lot of these metrics being obtained by the same organizations, many of them did not have universalized country names. For example, The United Kingdom sometimes showed up as Great Britain, or the UK.  To combat this, I installed and imported "country_converter". This didn't fix all the issues, but it did limit how many countries I was inadvertently losing due to attempting to merge data frames with non-matching names.

The datasets I was able to obtain did not have a large number of overlapping years. That said, I did my best to filter each dataset down to the most recent years with sufficient measurements. All datasets come from a ten year period of time (2015 - 2025).


Technologies Used
Python / Pandas - for exploration, normalizing and aggregation of the dataset
Tableau - for creating interactive dashboard
Figma - for introduction of Project
Canva - for introduction of Project
Git - for version control
Data Sources
To answer the above questions I used the following sources to collect datasets for my analysis:
[Basic Water](https://ourworldindata.org/grapher/population-using-at-least-basic-drinking-water)
[Basic Sanitation](https://ourworldindata.org/grapher/share-using-safely-managed-sanitation)
[Life Expectancy](https://ourworldindata.org/grapher/life-expectancy-hmd-unwpp?tab=table)
[Pollution](https://ourworldindata.org/grapher/pm25-air-pollution)
[Insufficient Calories](https://ourworldindata.org/grapher/number-calorie-diet-unaffordable)
[Unemployment](https://ourworldindata.org/grapher/unemployment-rate)
[Terrorist Attacks](https://ourworldindata.org/grapher/terrorist-attacks)
[Functioning Government Index](https://ourworldindata.org/grapher/functioning-government-index-eiu)
[Crime Rate](https://worldpopulationreview.com/country-rankings/crime-rate-by-country)
[Universal Healthcare Index](https://ourworldindata.org/grapher/universal-health-coverage-index)
[Atkinson Inequality Index](https://ourworldindata.org/grapher/income-inequality-atkinson-index-undp)
[Equal Rights Protection Index](https://ourworldindata.org/grapher/equal-rights-protection-index)
[Years of Schooling](https://ourworldindata.org/grapher/mean-years-of-schooling-long-run)
[Depression Rates](https://ourworldindata.org/grapher/depressive-disorders-prevalence-ihme)
[LGBT+ Equality Index](https://ourworldindata.org/grapher/lgbt-legal-equality-index)
[Suicides per 100k](https://ourworldindata.org/suicide)




Conclusion

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