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
- On a statewide basis from 1980-2000, are there any discernible trends with regard to ticket-splitting in Tennessee? How does the data compare by decade? Were there sudden partisan shifts or did they occur gradually?
- Since 2000, what are the county-level trends with regard to ticket-splitting? Do they mirror the same patterns that are seen statewide? How many counties, if any, have split their ticket in recent elections?
- Are voters more likely to split their ticket depending on the office?
- Have certain demographic groups (age, race, level of education, occupation) been more likely to split their tickets? If so, which ones and to what extent?

Known Issues and Challenges

Data Sources
Tennessee Secretary of State:
 - All TN election results 1998-2020 (down to precinct level) [1998-2006 (PDF); 2008-2020 (Excel)]

Harvard Dataverse:
 - All TN election results 2002 (down to precinct level)
 - All TN election results 2004-2006 (down to precinct level)
 - US President election results 1976-2020 (state level)
 - US President election results 1976-2020 (county level)
 - US Senate election results 1976-2020 (state level)
 - US House election results 1976-2020 (by cong. district)
 - All US State Legislature election results 1967-2016

US Election Atlas:
 - TN Gubernatorial election results 1974-2018 (state level)

US Census:
 - County & District shapefiles

Census Reporter:
 - US Census Demographics Data (2020)


Tools
 - Python, version 3.9.7 (default, Sep 16 2021, 16:59:28) [MSC v.1916 64 bit (AMD64)] (pandas, matplotlib, seaborn)
 - Jupyter Notebook, version 6.4.5
 - MS Excel, Microsoft 365
 - MS PowerPoint, Microsoft 365