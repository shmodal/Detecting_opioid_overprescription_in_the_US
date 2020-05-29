# Detecting opioid overprescription in the US

The US suffers from an opioid epidemic, in which there is an extensive overuse of opioid drugs (10.8M
people misused opioid prescriptions in 2018). There are large costs of this including loss of lives, health
care, criminal justice, and lost economic productivity. Our objective will be to identify pharmacies that
have filled an excessive number of opioid prescriptions in the states of Kentucky, Tennessee, and West
Virginia between the years 2006 and 2012. This will point to pharmacies who may be illegally distributing
opioids or neighboring doctors who overprescribe opioids. It is also a proxy for understanding which areas
are suffering the most opioid abuse. Thus, we aim to inform senior decision-makers (1) which pharmacies
should be investigated for potential malpractice and (2) which counties to focus interventions on.


The main data source is the [Automation of Reports and Consolidated Orders System (ARCOS)](https://d2ty8gaf6rmowa.cloudfront.net/dea-pain-pill-database/bulk/arcos_all_washpost.tsv.gz)
which was established by the Drug Enforcement Agency (DEA). The dataset tracks the path of every opioid pain pill
(oxycodone and hydrocodone), from manufacturer to pharmacy, in the United States between 2006 and
2012. Also, secondary sources of data used are [US census data](https://factfinder.census.gov/) (population, age, income, population), 
and [health indicators](https://www.countyhealthrankings.org) (percentage insured and number of physicians per county)

Methods used :

(1) Visualization - Calculate metrics such as number of pills purchased per capita at the zip code
level and visualize on heat maps.
(3) Time series - Graph trend lines to study the rate of opioid purchases by individual pharmacies. A
peak in the rate of opioid purchases may indicate the pharmacy has started to oversell opioids.
(2) Clustering - Cluster pharmacies based on demographics, density of pharmacy in the areas,
number of doctors, and other external environmental factors. This serves as a proxy for regrouping pharmacies with a similar market for opioid pills.
Within each group of similar pharmacies, we looked for outliers in number of sales.

