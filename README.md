# ELECTION ANALYSIS

## Project Overview
A Colorado Board of Elections official has requested an election audit of a recent local congressional election. The election audit will include a vote count report that will be used to certify the election. From the data provided, the vote count report will:

1. Calculate the total number of votes cast.
2. Calculate the total voter turnout for each county.
3. Calculate the percentage of votes from each county out of the total count.
4. Determine the county with the highest turnout.
5. Get a complete list of candidates who received votes.
6. Calculate the total number of votes each candidate received.
7. Calculate the percentage of votes each candidate won.
8. Determine the winner of the election based on the popular vote.

## Results
A total of 369.711 votes were cast in the congressional election.
### Results by County
- Jefferson County - 38,855 votes (10.5% of total votes)
- Denver County - 306,055 votes (82.8% of total votes)
- Arapahoe County - 24,801 votes (3.1% of total votes)
### Results by Candidate
- Charles Casper Stockham - 85,213 votes (23.0% of total votes)
- Diana DeGette - 272,892 votes (73.8% of total votes)
- Raymon Anthony Doane - 11,606 votes (3.1% of total votes)

### ELECTION WINNER: Diana DeGette with 272,892 votes - 73.8% of all votes

## Summary
The script used in the analysis could be applied to future elections with minor modification. First, the the script must be updated to load the appropriate file. As written, the script can open and read only the provided file or files with the same name. This would require an update to the current script in line 9 (below).

file_to_load = os.path.join("Resources", "election_results.csv")

In addition, the name of the output text file should be updated to reflect the type/name of the election. This would require changing the current script in line 11 (below).

file_to_save = os.path.join("analysis", "election_analysis.txt")

Finally, the current script writes results by county. Depending on the scope of the election the script should be updated to display results based on a different geographical areas (e.g., district, city, state). This can be accomplished by updating lines 88 and 114 in the code. Alternatively, the script could be updated to pull this information from cell B1 in the source file to eliminate hard-coded values.

## Resources
- Data Source: election_results.csv
- Software: Python 3.7.6, Visual Studio Code
