# Share of the population living in urban areas - Data package

This data package contains the data that powers the chart ["Share of the population living in urban areas"](https://ourworldindata.org/grapher/share-of-population-urban?v=1&csvType=full&useColumnShortNames=false) on the Our World in Data website. It was downloaded on April 12, 2025.

### Active Filters

A filtered subset of the full data was downloaded. The following filters were applied:

## CSV Structure

The high level structure of the CSV file is that each row is an observation for an entity (usually a country or region) and a timepoint (usually a year).

The first two columns in the CSV file are "Entity" and "Code". "Entity" is the name of the entity (e.g. "United States"). "Code" is the OWID internal entity code that we use if the entity is a country or region. For normal countries, this is the same as the [iso alpha-3](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-3) code of the entity (e.g. "USA") - for non-standard countries like historical countries these are custom codes.

The third column is either "Year" or "Day". If the data is annual, this is "Year" and contains only the year as an integer. If the column is "Day", the column contains a date string in the form "YYYY-MM-DD".

The final column is the data column, which is the time series that powers the chart. If the CSV data is downloaded using the "full data" option, then the column corresponds to the time series below. If the CSV data is downloaded using the "only selected data visible in the chart" option then the data column is transformed depending on the chart type and thus the association with the time series might not be as straightforward.

## Metadata.json structure

The .metadata.json file contains metadata about the data package. The "charts" key contains information to recreate the chart, like the title, subtitle etc.. The "columns" key contains information about each of the columns in the csv, like the unit, timespan covered, citation for the data etc..

## About the data

Our World in Data is almost never the original producer of the data - almost all of the data we use has been compiled by others. If you want to re-use data, it is your responsibility to ensure that you adhere to the sources' license and to credit them correctly. Please note that a single time series may have more than one source - e.g. when we stich together data from different time periods by different producers or when we calculate per capita metrics using population data from a second source.

## Detailed information about the data


## Urban population (% of total population)
Last updated: January 24, 2025  
Next update: January 2026  
Date range: 1960–2023  
Unit: % of total  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
UN Population Division (via World Bank) (2025) – processed by Our World in Data

#### Full citation
UN Population Division (via World Bank) (2025) – processed by Our World in Data. “Urban population (% of total population)” [dataset]. UN Population Division (via World Bank), “World Development Indicators” [original data].
Source: UN Population Division (via World Bank) (2025) – processed by Our World In Data

### How is this data described by its producer - UN Population Division (via World Bank) (2025)?
Urban population refers to people living in urban areas as defined by national statistical offices. The data are collected and smoothed by United Nations Population Division.

Limitations and exceptions: Aggregation of urban and rural population may not add up to total population because of different country coverage. There is no consistent and universally accepted standard for distinguishing urban from rural areas, in part because of the wide variety of situations across countries.

Most countries use an urban classification related to the size or characteristics of settlements. Some define urban areas based on the presence of certain infrastructure and services. And other countries designate urban areas based on administrative arrangements. Because of national differences in the characteristics that distinguish urban from rural areas, the distinction between urban and rural population is not amenable to a single definition that would be applicable to all countries.

Estimates of the world's urban population would change significantly if China, India, and a few other populous nations were to change their definition of urban centers.

Because the estimates of city and metropolitan area are based on national definitions of what constitutes a city or metropolitan area, cross-country comparisons should be made with caution.

Statistical concept and methodology: Urban population refers to people living in urban areas as defined by national statistical offices. The indicator is calculated using World Bank population estimates and urban ratios from the United Nations World Urbanization Prospects.

Percentages urban are the numbers of persons residing in an area defined as ''urban'' per 100 total population. Particular caution should be used in interpreting the figures for percentage urban for different countries.

Countries differ in the way they classify population as "urban" or "rural." The population of a city or metropolitan area depends on the boundaries chosen.

### Source

#### UN Population Division (via World Bank) – World Development Indicators
Retrieved on: 2025-01-24  
Retrieved from: https://datacatalog.worldbank.org/search/dataset/0037712/World-Development-Indicators  


    