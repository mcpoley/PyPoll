
# PyPoll Report

## Overview of Method

For the upcoming congressional election in Colorado, the election board has been tasked with auditing the election turn-out in terms of total votes cast, total votes per candidate, vote percentage per candidate, and overall winner. The voting methods taken into consideration were mail in ballots, direct recording electronic, and punch cards. In a similar manner, the board was also asked to find the same summary voting information for each county. An automated process used to tabulate these results can be done with Python via "for" loops. Once this code was formatted for the congressional district elections, it was saved for alternate future election use.


## Results

o	In their analysis, the election team discovered that a total 369, 711 votes were cast. This was determined by setting a total vote-count to zero, adding by one each time through the loop:

total_votes=0
total_votes=total_votes+1

o	A breakdown of votes and percentages per each county can be shown in the following image:
![image](https://github.com/mcpoley/PyPoll/blob/main/county_summary.png)

o	The county which received the largest number of votes ended up being Denver, with 306, 055 (82.8%) of the votes.

o	A breakdown of total votes per candidate and percentages can be shown with the following image:
![image](https://github.com/mcpoley/PyPoll/blob/main/candidate_summary.png)



o	The winner of the election ended up being Diana DeGette with 272, 892 (73.8%) of the total. 


## Summary
Fortunately, the script for the election committee need not be altered by a lot for future election summary. The first "for" loop deals with looping through the rows of a csv file. This part would generally work for any election, except for the particular rows being looped. For instance, Candidate_name would always work as a variable no matter what election, only the row number would be different depending on the file. The candidate summary information would probably be fine as is since each election requires a winning candidate. However, the general region considered would change. The “county” variable could then be changed to “city” or “state”. With these two small changes, the rest of the code could work for a variety of election uses. 
