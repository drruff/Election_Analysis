# Election_Analysis

## Project Overview
A Colorado Board of Elections employee has given you the following tasks to complete the election audit of a recent local congressional eleciton.

1. Calculate total number of votes
2. Get a complete list of candidates who recieved votes
3. Calculate a total number of votes each candidate recieved.
4. Calculate the precentage of votes each candidate won.
5. Determine the winner of the election based upon popular votes

## Resources
- Data sourceL election_results.csv
- Software: python 3.7.6, Visual Studio Code 1.623


## Summary
The analysis of the election shows that:
- There were total votes: 369,711
- The candidates were:
  - 1. Charles Casper
  - 2. Diana DeGette
  - 3. Raymon Anthony Doane
 
- The candidate results were:
  - 1. Charles Casper recieved "23.0%" of the vote, with "85,213" number of votes
  - 2. Diana DeGette recieved "73.8%" of the vote, with "272,892" number of votes
  - 3. Raymon Anthony Doane recieved "3.1%" of the vote, with "11,606" number of votes

- The winner of the election was: 
  - Diana DeGette recieved "73.8%" of the vote, with "272,892" number of votes


## Challenge Overview
A Colorado Board of Elections employee has given you the additional following tasks to complete the election audit of a recent local congressional eleciton, regarding the information on the cuonties of the region

1. How many votes were cast in this congressional election?
2. Provide a breakdown of the number of votes and the percentage of total votes for each county in the precinct.
3. Which county had the largest number of votes?
4. Provide a breakdown of the number of votes and the percentage of the total votes each candidate received.
5. Which candidate won the election, what was their vote count, and what was their percentage of the total votes?

## Challenge Summary
- There were total votes: 369,711
- The counties, and their results were:
  - Jefferson recieved "10.5%" of the vote, with "38,855" number of votes
  - Denver recieved "82.8%" of the vote, with "306,055" number of votes
  - Arapahoe recieved "6.7%" of the vote, with "24,801" number of votes
- The County with the largest turnout
  - Denver recieved "82.8%" of the vote, with "306,055" number of votes

- The candidate results were:
  - 1. Charles Casper recieved "23.0%" of the vote, with "85,213" number of votes
  - 2. Diana DeGette recieved "73.8%" of the vote, with "272,892" number of votes
  - 3. Raymon Anthony Doane recieved "3.1%" of the vote, with "11,606" number of votes

- The winner of the election was: 
  - Diana DeGette recieved "73.8%" of the vote, with "272,892" number of votes

This code can ultimately used to do this type of analysis with any election, as long as it is modified appopriately.
The follwoing is two ways the code can be modified to used in different elections:
- We change the type of election from say congressional to city:
  - We would simply change the "county" variable names to "district" variable names.
- We can change the type of voting from single vote to ranked voting (where we vote rank all candidates from most to least prefered to win): 
  - We would need to create a list that keeps track of the the "least amount of votes" for each round of counting, then add an if statement that only counts the most preffered vote for each person as long as they are not in this list.
  - This is assuming the data is kept similar the data we are presented here, but the most prefered is the lowest numbered column, and thus the if statement just changes row[2] to row[x] where x=2+p, where p=number of preffered votes in the least amount of votes list, thus taking the next most prefered vote.
