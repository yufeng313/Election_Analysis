# Election_Analysis
Automate election analysis using Python
## Overview of Election Audit
In this project, we will automate election audit using Python instead of Excel, to count the votes and get the final election results for U.S Congressional precinct in Colorado.<br/>
Except for the total number and percentage of votes for each candidate, and the winner of election based on the popular vote, we still need to know the information about the voter turnout for each country and the county with the highest turnout. So in this challenge. I'll use Python code to analyze the election results, and then provide a written analysis of the election audit for the election commission.
## Resources
Data source: election_results.csv<br/>
Software: Python 3.9.12  Visual Studio Code 1.68.1
## Election Audit Results
I wrote a script to retrieve the data from the given CSV file, used loops and conditional statements to calculate the county’s total vote count and the percentage of votes for the county. Here are some parts of the code:<br/>
1. Get the county name from CSV file, and calculate the county's vote count. Create a county dictionary to hold these data.<br/>
![produce county list and dictionary](https://user-images.githubusercontent.com/107179765/176630969-b23e34b9-9f85-4793-ae05-9ed048f5d7e0.png)<br/>
2. Write a for loop to get the county votes from the county dictionary. Calculate the percentage of votes for the county. Determine the winning county and get its vote count.<br/>
![analysis for county votes](https://user-images.githubusercontent.com/107179765/176631003-2bd7e7d2-688b-4382-a53f-b57ad31b7219.png)<br/>
3. Write the results to a text file.<br/>
![election results](https://user-images.githubusercontent.com/107179765/176631221-792063f5-c88f-4720-8b9f-a838c131f64d.png)<br/>
From the analysis results we can see that:<br/>
- There are 369,711 votes cast in the election.<br/>
- The number of votes and the percentage of total votes for each county in the precinct:
  - Jefferson county had 10.5% of voters, for a total of 38,855 voters.
  - Denver county had 82.8% of voters, for a total of 306,055 voters.
  - Arapahoe county had 6.7% of voters, for a total of 24,801 voters.
-	Denver county had the largest number of votes.
-	The number of votes and the percentage of the total votes each candidate received:
    -	Charles Casper Stockham received 23.0% of the vote, for a total of 85,213 votes.
    -	Diana DeGette received 73.8% of the vote, for a total of 272,892 votes.
    -	Raymon Anthony Doane received 3.1% of the vote, for a total of 11,606 votes.<br/>
-	Diana DeGette is the winner of this election, who received 73.8% of the vote, for a total of 272,892 votes.
## Election Audit Summary
In Colorado election audit, it’s easy to get the audit results which we need from the script. Actually this script can also be used in calculation for any election with some modifications in the future.<br/> 
For example, if we want to know what the percentages of each county voted for each candidate, we can add more code to group the candidate by the county first, and then do the same calculations with a little modifications on this script.<br/>
When it comes to bigger precinct, let’s say state-level or federal election, this script can also be used to run the results.<br/>
Since there are 3 primary voting methods need to be taken into account: Mail-in ballots, punch cards, and DRE counting machines, we can also use the script to count the total votes on each method to get the final results, and even found out which method is the most popular voting method in each county.<br/>
So, no matter what numbers of counties and candidates in an election, we can always use this script with some modifications to run the election analysis.
