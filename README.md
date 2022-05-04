# election_analysis

## Overview of Election Audit

 For this project, we focused on analysing the results of a local senate election in Colorado for the Colorado Board of Elections. Essentially, we have the raw data in the form of a CSV (comma-separated values) file. With this CSV file, our task was to find several pieces of information: the total number of votes cast, the list of candidates in the election who received votes, the number of votes each candidate received, the percentage of votes each candidate received, the winner of the election based on popular vote, voter turnout for each county, percentage of total votes from each county, and the county with the highest voter turnout. This was quite a lot of values to find, so we also needed to organize these all into an output text file that was easy to read and understand. This output file and the whole of our analysis will help the Colorado Board of Elections

## Election-Audit Results

 The results of our analysis can be seen in the image below, which is a screenshot of the text file output of our code:

![image](https://user-images.githubusercontent.com/103055666/166803828-db60fd97-a4d2-41c6-a84b-ddd81d9cf16c.png)

* How many votes were cast in this congressional election?
    * There were 369,711 votes cast in the election. 

* Provide a breakdown of the number of votes and the percentage of total votes for each county in the precinct.
    * There were three counties that participated in the senate election: Jefferson, Denver, and Arapahoe. Jefferson County had 38,855 votes, which made up 10.5% of the total vote distribution by county. Denver had 306,055 votes, making up 82.8% of the vote distribution. Arapahoe County had 24,801 votes, making up 6.7% of the vote distribution.

* Which county had the largest number of votes?
    *   Denver had 306,055 votes, making it have the largest share of votes per county. It made up 82.8% of the total vote count.

* Provide a breakdown of the number of votes and the percentage of the total votes each candidate received.
    * Charles Casper Stockham had 85,213 votes, making up 23.0% of the vote distribution by candidate. Diana DeGette had 272,892 votes, making up 73.8% of the vote distribution. Raymond Anthonay Doane had 11,606 votes, making up 3.1% of the vote distribution. 

* Which candidate won the election, what was their vote count, and what was their percentage of the total votes?
    * Diana DeGette won the election with 272,892 votes, or 73.8% of the total vote count.
    
## Election-Audit Summary

"In a summary statement, provide a business proposal to the election commission on how this script can be used—with some modifications—for any election. Give at least two examples of how this script can be modified to be used for other elections."

While we developed this script to return the results specifically for this election, it can certainly be used with slight modifications in other elections. An examples of a modification needed to examine a different election would be the below screenshot:

<img width="528" alt="Screen Shot 2022-05-04 at 3 36 24 PM" src="https://user-images.githubusercontent.com/103055666/166812481-14e7efbe-3f7c-447c-a6ef-209abc17a11d.png">

We would have to adapt this piece of the code that appears early in the script because it tells this script to go into the files containing the raw data on this specific election. To have this script run on a different election results file, we'd have to change this piece of the code to go into a different file containing election results for a different election.

Another thing we'd have to consider when using this script on another election is what kind of election we will be analysing. For example, if we were running this code on a nation-wide election, we'd probably be more interested in results per state than results per county. The below piece of the script would have to be changed:

<img width="499" alt="Screen Shot 2022-05-04 at 3 41 35 PM" src="https://user-images.githubusercontent.com/103055666/166813272-a6edde85-bd02-453b-a765-0e6176ec3694.png">

This is a snippet of code where we define a list and dictionary for the counties involved in the election. This owul dhave to be changed to something along the lines of "state_names = []" and "state_votes = {}." This would make it less confusing while coding the script to work for nationwide elections.
