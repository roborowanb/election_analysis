# election_analysis
Using Python to collect election results
## Overview of Election Results
Tom is looking for fast and reliable programming to help tally the election results. Luckily for Tom, python can be used to wiz through data. In this example, we will be looking at the counties; Jefferson, Denver, and Arapahoe. And candidates; Charles Casper, Diana DeGette, and Raymon Anthony Doane. We will aim to get the voter turnout for each country, the percentage of votes from each county out of the total count, and the county with the highest turnout. Lets see the results. 


## Election Audit Results


Total Votes: 369,711<br />


County Votes:<br />
Jefferson: 10.5% (38855)<br />
Denver: 82.8% (306055)<br />
Arapahoe: 6.7% (24801)<br />

Largest voter turnout: Denver<br />
Voters: 306055<br />

Charles Casper Stockham: 23.0% (85,213)<br />
Diana DeGette: 73.8% (272,892)<br />
Raymon Anthony Doane: 3.1% (11,606)<br />

Winner: Diana DeGette<br />
Winning Vote Count: 272,892<br />
Winning Percentage: 73.8%<br />

* The total votes casted were 369,711 votes
* Denver had the largest voter turnout
* Diana Degette won the election with 73.8% of the votes, exactly 272,892 votes were casted towards her


## Election Audit Summary
The great thing about this code is that it can be resused in any election, for any county, with any candidates. By using the code below, the script will acknowledge any new name that is not already in the list and immediately add it to the list before giving it its voter count. 

        if candidate_name not in candidate_options:
            candidate_options.append(candidate_name)
            candidate_votes[candidate_name] = 0
        candidate_votes[candidate_name] += 1
        
The same can be done with countys.
       
       if county_name not in county_list:
            county_list.append(county_name)
            county_votes[county_name] = 0
        county_votes[county_name] +=1

By creating dynamic a list, the script can be reused with no rework required!
