# Election Results Analysis

## Overview of Project

### Purpose

The purpose of this election audit analysis is to provide the election commission with some additional information as a follow-up to our audit of the election results. This report will complete the audit by providing the; _voter turnout for each county, percentage of votes from each county out of the total count and county with the highest turnout_. To complete this analysis, the election results csv that was provided by the commission was analyzed and requested results have been printed to the terminal command line and our election results text file. Below is a written analysis of county results with an overview of methods used and an election-audit summary with how this script (with modifications) might be used for other elections. 

## Election-Audit Results

- **How many votes were cast in this congressional election?**

In this congressional election, 369,711 votes were cast across three counties. 
##### Total votes printed to the command line and saved to the text file
>
In order to accurately report on the total votes, a counter (_total_votes_) was initialized and set to zero. As each row was read by the reader, the total vote count was increase by 1 and printed to the command line, as well as save to the text file.
##### _total_votes_ declared and set to 0.
>
##### _total_votes_ count increased by 1 as the loop went through each row.
>
##### _total_votes_ reported.
>

- **Provide a breakdown of the number of votes and the percentage of total votes for each county in the precinct.**

The number total number of votes and percentage of total votes was recorded for each county in the precinct. The results are as follows:
  - Jefferson: 10.55 (38,855)
  - Denver: 82.8% (306,055)
  - Arapahoe: 6.7% (24,801)
These results were tracked by capturing and adding each county to the county list and counting each vote reported for that county. The vote counts for each county were used to calculate and report on the percentage of votes for each county. 
##### Recording each county and number of votes for those counties.
>
##### Calculating the percentage of votes for the county and printing the results to the command line, as well as saving them to the text file.
>

- **Which county had the largest number of votes?**

The county that had the largest number of votes was Denver with 82.8% of votes (306,055). Each county's total vote count was reviewed by the script and the county with the largest total was reported in the command line and saved to the text file. 
##### Winning county was determined and reported.
>

- **Provide a breakdown of the number of votes and the percentage of the total votes each candidate received.**

The total number of votes and percentage of votes was reported for each candidate as follows:
  - Charles Casper Stockham: 23.0% (85,213)
  - Diana DeGette: 73.8% (272,892)
  - Raymon Anthony Doane: 3.1% (11,606)
For each candidate, their total vote count was retrieved and divided by the total votes to calculate the percentage of votes they received. These results were reported in the command line and saved to the text file. 
##### Candidate votes retrieved and percentage calculated.
>
##### Candidate results were reported.
>

- **Which candidate won the election, what was their vote count, and what was their percentage of the total votes?**

Diana Degette was the candidate that won the election according to our audit, with 73.8% of votes (272,892). We were able to accurately report the winner by comparing the total votes for each candidate within the _candidate_votes_ dictionary within the script. These results were then recorded in the command line and saved to the text file. 
##### Candidate total votes were compared and the winning candidate was identified.
>
##### Winning candidate results were reported. 
>

## Election-Audit Summary

The business proposal to the election commission includes two examples of how this script, with modifications, can be used for future elections. 
  1. Rather than running two loops that are hard coded to report only on candidate and county data, the script can be modified to capture and report on multiple columns utilizing the heading titles. The header variable would be used to create lists and dictionaries for each column heading that could be accessed to provide summaries on the results. 
  1. Additional analyses could be included to calculate what percentage of a county's population voted. If we were to include data on each county's population, we could divide each county's total vote count by this number to report on voter turn out. This information is beneficial to the commission to identify counties that have low voter turnout and potentially implement programs to increase these numbers. 
