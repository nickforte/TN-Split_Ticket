Analysis of Ticket Splitting in Tennessee Elections, 1980-2020
Capstone Project for Nashville Software School Daytime Data Analytics Cohort #6

Table of Contents
 - Motivation
 - Data Questions
 - Known Issues and Challenges
 - Data Sources
 - Tools

Motivation
As a Nashville native, I’ve seen Tennessee’s political landscape change considerably over my lifetime – 35 years and counting. From 1980 to 2000 neither major party could claim electoral dominance – the electorate showed a clear willingness to elect (and re-elect) Republican and Democratic candidates alike, regardless of office. Both Republicans and Democrats won Presidential elections, Gubernatorial races, and U.S. Senate seats, and state’s congressional delegation remained fairly balanced between the two parties.

Elections seemingly weren’t decided based purely on partisanship, evidenced by several election cycles where Tennesseans elected candidates from both parties on the same ballot. For example, in 1982 a Democrat won a U.S. Senate seat while a Republican won the gubernatorial race. This wasn’t an uncommon occurrence, and it was clear evidence that a relatively substantial percentage of voters were open to split-ticket voting or “ticket splitting” – voting for candidates of opposing political parties on the same ballot, in contrast to voting for a straight one-party ticket.

An obvious shift occurred between 2000 and 2010 however; no Democrat has won a statewide election since 2006, and Republicans have dominated both the congressional delegation and the state legislature since 2010. I’m fascinated by this relatively recent shift, and I want to explore how it correlates with ticket splitting, or potentially the lack of ticket splitting . Additionally, I want to explore whether ticket splitting is more common for certain offices, and whether certain demographics (age, race, income, education) are more likely to split their ticket.

Data Questions
- On a statewide basis from 1980-2000, are there any discernible trends with regard to ticket-splitting in Tennessee? How does the data compare by decade? Did any partisan shifts occur suddenly or more gradually?
- Since 2000, what are the county-level trends with regard to ticket-splitting? Do they mirror the same trends that are seen statewide? How many counties, if any, have split their ticket in recent elections?
- Do certain offices see more ticket splitting than others? Has this changed over time?
- Have certain demographic groups (age, race, level of education, occupation) been more likely to split their tickets? If so, which ones and to what extent?

Known Issues and Challenges
Finding all the data I wanted to use was more difficult than I anticipated. The TN Secretary of State website contains results down to the precinct-level in Excel spreadsheets, but only going back to 2008, so I relied on the Harvard Dataverse for county-level results from 2002-2006, as well as state-level results and state legislature results from 1980-2020. However I was still lacking state-level Gubernatorial election results from 1980-1998, so I scraped these results from the US Election Atlas. Unfortunately I wasn't able to find county-level results for anything other than Presidential Elections from 1980-2000, so I decided to limit my county-level analysis to the past 10 election cycles (2002-2020). The Census data was pretty easy to find but there was a lot of it, so figuring out which data I wanted to use was the only challenge there.

Once I had all my data in hand, cleaning it proved to be another significant challenge. Practically every data source I used had election results formatted differently, so I spent nearly a week cleaning all my data in order to build a Statewide Master Table with results from 1980-2020, and a County Master Table with results from 2002-2020. From there I joined the county shapefiles and Census data with the County Master Table, and then I was able to begin analyzing my data.

Data Sources
Tennessee Secretary of State:
 - All TN election results 1998-2020 (down to precinct level) https://sos.tn.gov/elections/results

Harvard Dataverse:
 - All TN election results 2002 (down to precinct level) https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/YN4TLR
 - All TN election results 2004-2006 (down to precinct level) https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/YN4TLR
 - US President election results 1976-2020 (state level) https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/42MVDX
 - US President election results 1976-2020 (county level) https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/VOQCHQ
 - US Senate election results 1976-2020 (state level) https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/PEJ5QU
 - US House election results 1976-2020 (by cong. district) https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/IG0UN2
 - All US State Legislature election results 1967-2016 https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/DRSACA

US Election Atlas:
 - TN Gubernatorial election results 1974-2018 (state level) https://uselectionatlas.org/RESULTS/compare.php?year=1982&fips=47&f=0&off=5&elect=0&type=state

US Census:
 - County & District shapefiles https://www.census.gov/cgi-bin/geo/shapefiles/index.php

Census Reporter:
 - US Census Demographics Data (2020) https://censusreporter.org/profiles/04000US47-tennessee/

Tools
 - Python, version 3.9.7 (pandas, numpy, matplotlib, seaborn)
 - Jupyter Notebook, version 6.4.5
 - MS Excel, Microsoft 365
 - MS PowerPoint, Microsoft 365
