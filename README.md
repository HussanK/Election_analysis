# Election_analysis

## Overview of Prject

The purpose of this project was to gain basic understanding of Python, and how to uise Python to read and interpret data given in a CSV format. Many of the skills required to 
complete this challenge can easily be transferred to analyzing data from CSVs in the real world. Not only that this has further our understanding of coding logic, something that 
is also easily transferrable into other aspects of a data driven carrer. Again we have been tasked with taking data that is hard for most people to understand, and putting it into
a format that is easily accessible. 

## Election-Audit Results 

 - There were 369,711 total votes cast during this election. 
 - Jefferson county had 10.5% of the vote with 38.885 votes, Denver County had 82.8% of the vote with 306,055 votes, and Arapahoe County had 6.7% of the vote with 11,606 votes.
 - Denver County had the most votes total. The way I was able to figure that out using code was a pretty simple if statement shown below: 
 ```
 if votes > highestTurnout:
             highestTurnout = votes
             largestCounty = county_name
 ```
 This if states compares the counties current number of votes (gained earlier in the for loop) against the higheset number gained so far, and if it is bigger it changes the
 variables I used for the amount of votes and name of the county with the most votes. 
 - Charles Casper Stockham recieved 85,213 votes which was 23%, Raymon Anthony Doane recieved 11,606 votes which was 3.1% and Diana DeGette recieved 272,892 votes which was 73.8%
 - This makes the winnner of the election Diana DeGette with 272,892 votes pr 73.8% of the total votes, a clear and decisive victor
 
 ## Election-Audit Summary
 
 Making this code was not only useful to interpret the data given to us in the election results csv, bust also this code can easily be refactored to fit any election data. The
 code itself doesn't directly use any specific names or variables to call out to the specific counties or candidates. Even if there are more or less counties or candidates the
 code itself would stil work. The only thing that would need to remain similar is the CSV of the data, and even then if the rows are out of order this can be easily changed. Only
 the code below would need to be change
 ```
  # Get the candidate name from each row.
        candidate_name = row[2]

        # 3: Extract the county name from each row.
        county_name = row[1]
```
and even with that all that would need to be changed are the numbers, which would need to correspond to the correct rows on the CSV. 
 
