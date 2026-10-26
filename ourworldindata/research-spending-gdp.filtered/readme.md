# Research & development spending as a share of GDP - Data package

This data package contains the data that powers the chart ["Research & development spending as a share of GDP"](https://ourworldindata.org/grapher/research-spending-gdp?v=1&csvType=filtered&useColumnShortNames=false) on the Our World in Data website. It was downloaded on October 23, 2026.

### Active Filters

A filtered subset of the full data was downloaded. The following filters were applied:

## CSV structure

Each row is an observation for an entity (usually a country or region) at a timepoint.

- "Entity" — the name of the entity, e.g. "United States".
- "Code" — our internal entity code. For most countries this is the [ISO alpha-3](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-3) code, e.g. "USA"; historical and other non-standard entities get a custom code.
- "Year" or "Day" — the timepoint. Annual data has a "Year" column holding an integer year; otherwise a "Day" column holds a date string in the form "YYYY-MM-DD".
- The final column is the data column — the time series that powers the chart. Downloaded with the "full data" option it corresponds to the time series below; with "only selected data visible in the chart" it is transformed depending on the chart type, so the correspondence may be less direct.

The data file includes an additional column suffixed with (Original Year) or (Original Day). This column appears when we use "tolerance" to display data for time points where exact data is unavailable. For example, if a country does not have data for one or more years, we use tolerance to fill the gaps using the closest available data points. These suffix columns show you which year (or day) the value really came from, allowing you to see when the data was actually measured.

## Metadata.json structure

The .metadata.json file contains metadata about the data package. The "charts" key contains information to recreate the chart, like the title, subtitle etc. The "columns" key contains information about each of the columns in the csv, like the unit, timespan covered, citation for the data etc.

## How we process data at Our World in Data

Our World in Data is almost never the original producer of the data - almost all of the data we use has been compiled by others. If you want to re-use data, it is your responsibility to ensure that you adhere to the sources' license and to credit them correctly. Please note that a single time series may have more than one source - e.g. when we stitch together data from different time periods by different producers or when we calculate per capita metrics using population data from a second source.

Preparing this data involves several processing steps. Depending on the data, this can include standardizing country names and world region definitions, converting units, calculating derived indicators such as per capita measures, as well as adding or adapting metadata such as the name or the description given to an indicator.
[Read about our data pipeline](https://docs.owid.io/projects/etl/).

## Detailed information about the data


### Research and development expenditure (% of GDP)
Last updated: July 27, 2026  
Next expected update: January 2027  
Date range: 1996–2024  
Unit: % of GDP  
Source: UNESCO UIS Stat Bulk Data Download Service, via World Bank (2026) – processed by Our World in Data  

#### How to cite this data

UNESCO UIS Stat Bulk Data Download Service, via World Bank (2026) – processed by Our World in Data

#### How this data is described by its producers
Gross domestic expenditures on research and development (R&D), expressed as a percent of GDP. They include both capital and current expenditures in the four main sectors: Business enterprise, Government, Higher education and Private non-profit. R&D covers basic research, applied research, and experimental development.

### Aggregation method:
Weighted average

### Statistical concept and methodology:
Methodology: This indicator is calculated by dividing the total domestic intramural expenditure on R&D for a given year by the gross domestic product (GDP) — defined as the sum of gross value added by all resident producers in the economy, including distributive trades and transport, plus any product taxes and minus any subsidies not included in the value of the products — and multiplying the result by 100.

Gross domestic expenditure on R&D (GERD) as a percentage of GDP (SDG Indicator 9.5.1) is the total intramural expenditure on R&D performed in the national territory during a specific reference period, expressed as a percentage of GDP of the national territory. Intramural R&D expenditures encompass all current expenditures plus gross fixed capital expenditures for R&D performed within a statistical unit during a specific reference period, regardless of the source of funds. The summation of intramural R&D expenditures across all sectors of the economy is equivalent to GERD.







Data are collected through national research and experimental development (R&D) surveys, either by the national statistical office or a line ministry (such as the Ministry for Science and Technology). The data compilers are the UNESCO Institute for Statistics (UIS), Organisation for Economic Co-operation and Development (OECD), Eurostat (Statistical Office of the European Union) and the Network on Science and Technology Indicators – Ibero-American and Inter-American (RICYT), African Science, Technology and Innovation (STI) Indicators Initiative (ASTII) of the African Union Development Agency-NEPAD (AUDA-NEPAD).
Statistical concept(s): The gross domestic expenditure on R&D indicator consists of the total expenditure (current and capital) on R&D by all resident companies, research institutes, university and government laboratories, etc. It excludes R&D expenditures financed by domestic firms but performed abroad.









The OECD's Frascati Manual defines research and experimental development as "creative work undertaken on a systemic basis in order to increase the stock of knowledge, including knowledge of man, culture and society, and the use of this stock of knowledge to devise new applications." R&D covers basic research, applied research, and experimental development.









(1) Basic research - Basic research is experimental or theoretical work undertaken primarily to acquire new knowledge of the underlying foundation of phenomena and observable facts, without any particular application or use in view









(2) Applied research - Applied research is also original investigation undertaken in order to acquire new knowledge; it is, however, directed primarily towards a specific practical aim or objective.









(3) Experimental development - Experimental development is systematic work, drawing on existing knowledge gained from research and/or practical experience, which is directed to producing new materials, products or devices, to installing new processes, systems and services, or to improving substantially those already produced or installed.









The fields of science and technology used to classify R&D according to the Revised Fields of Science and Technology Classification are:




1. Natural sciences;




2. Engineering and technology;




3. Medical and health sciences;




4. Agricultural sciences;




5. Social sciences;




6. Humanities and the arts.









The data are obtained through statistical surveys which are regularly conducted at national level covering R&D performing entities in the private and public sectors.

### Development relevance:
Science, technology, and innovation constitute pivotal elements for achieving sustainable growth. Sustainable Development Goal (SDG) target 9.5 is dedicated to the enhancement of scientific research and the advancement of technological capabilities within industrial sectors, with a particular focus on low- and middle-income countries. Furthermore, this target encompasses the objective of augmenting the cadre of research and development personnel, as well as escalating expenditures in research.

### Limitations and exceptions:
Estimates of the resources allocated to R&D are affected by national characteristics such as the periodicity and coverage of national R&D surveys across institutional sectors and industries; and the use of different sampling and estimation methods. R&D typically involves a few large performers, hence R&D surveys use various techniques to maintain up-to-date registers of known performers, while attempting to identify new or occasional performers.







R&D totals from SNA accounts may differ from these estimates, due in part to the different treatments of software R&D in the totals.


## Sources

These are the sources behind the data in this package. Each time series above names the ones it draws on in its citation.

### UNESCO UIS Stat Bulk Data Download Service, via World Bank – World Development Indicators

The World Development Indicators (WDI) database, published by the World Bank, is a comprehensive collection of global development data, providing key economic, social, and environmental statistics. It includes over 1,500 indicators covering more than 200 countries and territories, with data spanning several decades. WDI serves as a vital resource for policymakers, researchers, businesses, and analysts seeking to understand global trends and make data-driven decisions. The database covers a wide range of topics, including economic growth, education, health, poverty, trade, energy, infrastructure, governance, and environmental sustainability. The indicators are sourced from reputable national and international agencies, ensuring high-quality, consistent, and comparable data. Users can access the database through interactive online tools, API services, and downloadable datasets, facilitating detailed analysis and visualization. WDI is also used for tracking progress on the Sustainable Development Goals (SDGs) and other global development initiatives. By providing accessible and reliable statistics, it helps to inform policy discussions and strategies globally. Whether for academic research, policy planning, or economic analysis, the World Development Indicators database is an essential tool for understanding and addressing global development challenges.

Producer: UNESCO UIS Stat Bulk Data Download Service, via World Bank  
Published: 2026-07-15  
Retrieved on: 2026-07-27  
Retrieved from: https://data.worldbank.org/indicator/GB.XPD.RSDV.GD.ZS  
Direct download: https://databankfiles.worldbank.org/public/ddpext_download/WDI_CSV.zip  
License: CC BY 4.0 (https://datacatalog.worldbank.org/search/dataset/0037712/World-Development-Indicators)  

Citation: Stat Bulk Data Download Service, UN Educational, Scientific and Cultural Organization (UNESCO), uri: https://databrowser.uis.unesco.org/resources/bulk, publisher: UNESCO Institute for Statistics (UIS), date accessed: 2025-03-26, date published: 2025-02. Indicator GB.XPD.RSDV.GD.ZS (https://data.worldbank.org/indicator/GB.XPD.RSDV.GD.ZS). World Development Indicators – World Bank (2026). Accessed on 2026-07-27.

    