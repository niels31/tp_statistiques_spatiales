# Distribution of income across richer and poorer groups (before tax) - Data package

This data package contains the data that powers the chart ["Distribution of income across richer and poorer groups (before tax)"](https://ourworldindata.org/grapher/incomes-of-the-richest?v=1&csvType=full&useColumnShortNames=false&quantile=_10_40_50&welfare_type=before_tax) on the Our World in Data website.

### Active Filters

A filtered subset of the full data was downloaded. The following filters were applied:

## CSV structure

Each row is an observation for an entity (usually a country or region) at a timepoint.

- "Entity" — the name of the entity, e.g. "United States".
- "Code" — our internal entity code. For most countries this is the [ISO alpha-3](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-3) code, e.g. "USA"; historical and other non-standard entities get a custom code.
- "Year" or "Day" — the timepoint. Annual data has a "Year" column holding an integer year; otherwise a "Day" column holds a date string in the form "YYYY-MM-DD".
- Every remaining column is a data column, each one a time series. Downloaded with the "full data" option each corresponds to one time series below; with "only selected data visible in the chart" they are transformed depending on the chart type, so the correspondence may be less direct.


## Metadata.json structure

The .metadata.json file contains metadata about the data package. The "charts" key contains information to recreate the chart, like the title, subtitle etc. The "columns" key contains information about each of the columns in the csv, like the unit, timespan covered, citation for the data etc.

## How we process data at Our World in Data

Our World in Data is almost never the original producer of the data - almost all of the data we use has been compiled by others. If you want to re-use data, it is your responsibility to ensure that you adhere to the sources' license and to credit them correctly. Please note that a single time series may have more than one source - e.g. when we stitch together data from different time periods by different producers or when we calculate per capita metrics using population data from a second source.

Preparing this data involves several processing steps. Depending on the data, this can include standardizing country names and world region definitions, converting units, calculating derived indicators such as per capita measures, as well as adding or adapting metadata such as the name or the description given to an indicator.
[Read about our data pipeline](https://docs.owid.io/projects/etl/).

## Detailed information about each time series


### Richest 1%
Share of income received by the richest 1% of the population. Income here is measured before taxes and benefits.
Last updated: June 18, 2026  
Next expected update: June 2027  
Date range: 1820–2024  
Unit: %  
Source: World Inequality Database (WID.world) (2026) – with major processing by Our World in Data  

#### How to cite this data

World Inequality Database (WID.world) (2026) – with major processing by Our World in Data

#### What you should know about this data
- The data shows the share of total income received by different income groups. These income shares are measures of inequality: if incomes were equally distributed, each 1% of the population would receive 1% of total income. Inequality in the distribution of income is present when richer groups receive a more-than-equal share, and poorer groups receive less. We discuss these measures and the data in more detail on our page on [economic inequality](https://ourworldindata.org/economic-inequality).
- This data comes from the [World Inequality Database (WID)](https://wid.world/). This source has developed an approach to measuring inequality that aims to more accurately capture what is happening at the very top of the distribution, among the richest individuals. Traditional approaches, based on household survey data, tend to underestimate the incomes of the richest. WID tries to address this by combining data from tax records, surveys, and national accounts. You can read more about their method on our [page](https://ourworldindata.org/economic-inequality#tracking-the-incomes-of-the-richest-data-from-the-world-inequality-database).
- Before tax income is measured before taxes have been paid and most government benefits have been received. The exception is pensions and other social insurance benefits, such as unemployment insurance — contributions to these are deducted, and the corresponding benefits are added back as income. Read more.
- Income here refers to national income — a broad measure of income across the whole economy taken from the national accounts. This includes components of income not usually attributed to individuals, or that people wouldn't normally think of as part of their own income, such as retained corporate profits and imputed rent from owner-occupied housing.
- For some countries and years, the underlying data sources (household surveys, tax records) are not available. In these cases, WID estimates the missing values by extrapolating from other years or data from other countries, which introduces uncertainty. For more information, see the [WID methodology documentation](https://wid.world/document/distributional-national-accounts-dina-guidelines-2025-methods-and-concepts-used-in-the-world-inequality-database/).

#### Notes on our processing step for this indicator
We extract estimations of Gini, mean, percentile thresholds, averages, and shares via the [`wid` Stata command](https://github.com/world-inequality-database/wid-stata-tool). We calculate threshold and share ratios by dividing different thresholds and shares, respectively.

Interpolations and extrapolations are excluded by using the option `exclude` in the Stata command.


### Next 9%
Share of income received by the population between the 90th and 99th percentiles. Income here is measured before taxes and benefits.
Last updated: June 18, 2026  
Next expected update: June 2027  
Date range: 1820–2024  
Unit: %  
Source: World Inequality Database (WID.world) (2026) – with major processing by Our World in Data  

#### How to cite this data

World Inequality Database (WID.world) (2026) – with major processing by Our World in Data

#### What you should know about this data
- The data shows the share of total income received by different income groups. These income shares are measures of inequality: if incomes were equally distributed, each 1% of the population would receive 1% of total income. Inequality in the distribution of income is present when richer groups receive a more-than-equal share, and poorer groups receive less. We discuss these measures and the data in more detail on our page on [economic inequality](https://ourworldindata.org/economic-inequality).
- This data comes from the [World Inequality Database (WID)](https://wid.world/). This source has developed an approach to measuring inequality that aims to more accurately capture what is happening at the very top of the distribution, among the richest individuals. Traditional approaches, based on household survey data, tend to underestimate the incomes of the richest. WID tries to address this by combining data from tax records, surveys, and national accounts. You can read more about their method on our [page](https://ourworldindata.org/economic-inequality#tracking-the-incomes-of-the-richest-data-from-the-world-inequality-database).
- Before tax income is measured before taxes have been paid and most government benefits have been received. The exception is pensions and other social insurance benefits, such as unemployment insurance — contributions to these are deducted, and the corresponding benefits are added back as income. Read more.
- Income here refers to national income — a broad measure of income across the whole economy taken from the national accounts. This includes components of income not usually attributed to individuals, or that people wouldn't normally think of as part of their own income, such as retained corporate profits and imputed rent from owner-occupied housing.
- For some countries and years, the underlying data sources (household surveys, tax records) are not available. In these cases, WID estimates the missing values by extrapolating from other years or data from other countries, which introduces uncertainty. For more information, see the [WID methodology documentation](https://wid.world/document/distributional-national-accounts-dina-guidelines-2025-methods-and-concepts-used-in-the-world-inequality-database/).

#### Notes on our processing step for this indicator
We extract estimations of Gini, mean, percentile thresholds, averages, and shares via the [`wid` Stata command](https://github.com/world-inequality-database/wid-stata-tool). We calculate threshold and share ratios by dividing different thresholds and shares, respectively.

Interpolations and extrapolations are excluded by using the option `exclude` in the Stata command.


### Middle 40%
Share of income received by the middle 40% of the population. The middle 40% is the share of the population whose income lies between the poorest 50% and the richest 10%. Income here is measured before taxes and benefits.
Last updated: June 18, 2026  
Next expected update: June 2027  
Date range: 1820–2024  
Unit: %  
Source: World Inequality Database (WID.world) (2026) – with major processing by Our World in Data  

#### How to cite this data

World Inequality Database (WID.world) (2026) – with major processing by Our World in Data

#### What you should know about this data
- The data shows the share of total income received by different income groups. These income shares are measures of inequality: if incomes were equally distributed, each 1% of the population would receive 1% of total income. Inequality in the distribution of income is present when richer groups receive a more-than-equal share, and poorer groups receive less. We discuss these measures and the data in more detail on our page on [economic inequality](https://ourworldindata.org/economic-inequality).
- This data comes from the [World Inequality Database (WID)](https://wid.world/). This source has developed an approach to measuring inequality that aims to more accurately capture what is happening at the very top of the distribution, among the richest individuals. Traditional approaches, based on household survey data, tend to underestimate the incomes of the richest. WID tries to address this by combining data from tax records, surveys, and national accounts. You can read more about their method on our [page](https://ourworldindata.org/economic-inequality#tracking-the-incomes-of-the-richest-data-from-the-world-inequality-database).
- Before tax income is measured before taxes have been paid and most government benefits have been received. The exception is pensions and other social insurance benefits, such as unemployment insurance — contributions to these are deducted, and the corresponding benefits are added back as income. Read more.
- Income here refers to national income — a broad measure of income across the whole economy taken from the national accounts. This includes components of income not usually attributed to individuals, or that people wouldn't normally think of as part of their own income, such as retained corporate profits and imputed rent from owner-occupied housing.
- For some countries and years, the underlying data sources (household surveys, tax records) are not available. In these cases, WID estimates the missing values by extrapolating from other years or data from other countries, which introduces uncertainty. For more information, see the [WID methodology documentation](https://wid.world/document/distributional-national-accounts-dina-guidelines-2025-methods-and-concepts-used-in-the-world-inequality-database/).

#### Notes on our processing step for this indicator
We extract estimations of Gini, mean, percentile thresholds, averages, and shares via the [`wid` Stata command](https://github.com/world-inequality-database/wid-stata-tool). We calculate threshold and share ratios by dividing different thresholds and shares, respectively.

Interpolations and extrapolations are excluded by using the option `exclude` in the Stata command.


### Poorest 50%
Share of income received by the poorest 50% of the population. Income here is measured before taxes and benefits.
Last updated: June 18, 2026  
Next expected update: June 2027  
Date range: 1820–2024  
Unit: %  
Source: World Inequality Database (WID.world) (2026) – with major processing by Our World in Data  

#### How to cite this data

World Inequality Database (WID.world) (2026) – with major processing by Our World in Data

#### What you should know about this data
- The data shows the share of total income received by different income groups. These income shares are measures of inequality: if incomes were equally distributed, each 1% of the population would receive 1% of total income. Inequality in the distribution of income is present when richer groups receive a more-than-equal share, and poorer groups receive less. We discuss these measures and the data in more detail on our page on [economic inequality](https://ourworldindata.org/economic-inequality).
- This data comes from the [World Inequality Database (WID)](https://wid.world/). This source has developed an approach to measuring inequality that aims to more accurately capture what is happening at the very top of the distribution, among the richest individuals. Traditional approaches, based on household survey data, tend to underestimate the incomes of the richest. WID tries to address this by combining data from tax records, surveys, and national accounts. You can read more about their method on our [page](https://ourworldindata.org/economic-inequality#tracking-the-incomes-of-the-richest-data-from-the-world-inequality-database).
- Before tax income is measured before taxes have been paid and most government benefits have been received. The exception is pensions and other social insurance benefits, such as unemployment insurance — contributions to these are deducted, and the corresponding benefits are added back as income. Read more.
- Income here refers to national income — a broad measure of income across the whole economy taken from the national accounts. This includes components of income not usually attributed to individuals, or that people wouldn't normally think of as part of their own income, such as retained corporate profits and imputed rent from owner-occupied housing.
- For some countries and years, the underlying data sources (household surveys, tax records) are not available. In these cases, WID estimates the missing values by extrapolating from other years or data from other countries, which introduces uncertainty. For more information, see the [WID methodology documentation](https://wid.world/document/distributional-national-accounts-dina-guidelines-2025-methods-and-concepts-used-in-the-world-inequality-database/).

#### Notes on our processing step for this indicator
We extract estimations of Gini, mean, percentile thresholds, averages, and shares via the [`wid` Stata command](https://github.com/world-inequality-database/wid-stata-tool). We calculate threshold and share ratios by dividing different thresholds and shares, respectively.

Interpolations and extrapolations are excluded by using the option `exclude` in the Stata command.


## Sources

These are the sources behind the data in this package. Each time series above names the ones it draws on in its citation.

### World Inequality Database (WID.world) – World Inequality Database (WID)

The World Inequality Database (WID.world) aims to provide open and convenient access to the most extensive available database on the historical evolution of the world distribution of income and wealth, both within countries and between countries.

Producer: World Inequality Database (WID.world)  
Published: 2026  
Retrieved on: 2026-07-07  
Retrieved from: https://wid.world  
License: CC BY 4.0 (https://wid.world/)  

Citation: World Inequality Database (WID), https://wid.world

    