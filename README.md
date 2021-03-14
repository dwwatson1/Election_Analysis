# Election_Analysis
## Overview of Election Audit

A Colorado Board of Elections employee gave me the following tasks, split into two parts, to complete the election audit of a recent local congressional election.

**Part 1 - Audit of Results by Candidate**
1. Calculate the total number of votes cast.
2. Get a complete list of candidates who received votes.
3. Calculate the total number of votes each candidate received.
4. Calculate the percentage of votes each candidate won.
5. Determine the winner of the election based on popular vote.

**Part 2 - Audit of Results by County**
1. Calculate the total number of votes cast.
2. Get a complete list of counties that received votes.
3. Calculate the total number of votes each county received.
4. Calculate the percentage of votes is attributed to each county.
5. Determine the largest county turnout based on popular vote.

This audit will ensure votes are recorded and tallied accurately. In addition to the audit, my careful analysis will ensure the integrity of the vote the help the Colorado Board of Elections respond effectively to allegations of fraud and error.

## Part 1 - Audit of Results by Candidate
### Audit Resources
- Data Source: [election_results](https://github.com/dwwatson1/Election_Analysis/blob/main/Resources/election_results.csv)
- Software Python: Software: Python 3.7.6, Visual Studio Code, 1.38.1
- Script: [PyPoll](https://github.com/dwwatson1/Election_Analysis/blob/main/PyPoll.py)

### Election Audit Results
The analysis of the election showed that (also shown here [election_analysis](https://github.com/dwwatson1/Election_Analysis/blob/main/analysis/election_analysis.txt)):
- There were 369,711 votes cast in the election
- The candidates were
  - Charles Casper Stockham
  - Diana DeGette
  - Raymon Anthony Doane
- The candidate results were
  - Charles Casper Stockham received 23.0% of the vote with 85,213 votes
  - Diana DeGette received 73.8% received 73.8% of the vote with 272,892 votes
  - Raymon Anthony Doane received 3.1% of the vote with 11,606 votes
- The winner of the election was
  - **Diana DeGette received 73.8% of the vote with 272,892 votes**
 
To display Diana DeGette as the winning candidate with her vote count and winning percentage in the [election_analysis](https://github.com/dwwatson1/Election_Analysis/blob/main/analysis/election_analysis.txt) txt file, I ended the script with the follow f-string:

![Winning_Candidate](https://github.com/dwwatson1/Election_Analysis/blob/main/Resources/Winning_Candidate.PNG)

## Part 2 - Audit of Results by County
### Audit Resources
- Data Source: [election_results](https://github.com/dwwatson1/Election_Analysis/blob/main/Resources/election_results.csv)
- Software Python: Software: Python 3.7.6, Visual Studio Code, 1.38.1
- Script: [PyPoll_Challenge](https://github.com/dwwatson1/Election_Analysis/blob/main/PyPoll_Challenge.py)

### Election Audit Results
The analysis of the election showed that (also shown here [election_analysis](https://github.com/dwwatson1/Election_Analysis/blob/main/analysis/election_analysis.txt)):
- There were 369,711 votes cast in the election
- The counties were
  - Arapahoe
  - Denver
  - Jefferson
- The county results were
  - Arapahoe accounted 6.7% of the vote with 24,801 votes
  - Denver accounted 82.8% of the vote with 306,055 votes
  - Jefferson accounted 10.5% of the vote with 38,855 votes
- The largest county turnout was
  - **Denver accounted 82.8% of the vote with 306,055 votes**
  - 
To display Denver with the largest county turnout with hits vote count and turnout percentage in the [election_analysis](https://github.com/dwwatson1/Election_Analysis/blob/main/analysis/election_analysis.txt) txt file, I ended the script with the follow f-string:

![Winning_County](https://github.com/dwwatson1/Election_Analysis/blob/main/Resources/Winning_County.PNG)

## Election Audit Summary
### Application to Future Elections
The [PyPoll_Challenge](https://github.com/dwwatson1/Election_Analysis/blob/main/PyPoll_Challenge.py) Script can easily be modified to perform audits across all Colorado Congressional Districts or statewide elections, such as presidential, gubernatorial and Senate elections. I investigated the Colorado Secretary of State site for how they organize their [election data](https://results.enr.clarityelections.com/CO/105975/web.275533/#/summary?category=C_1). They have a category for contest name. If we added a column called __Contest Name__ we could extract data on statewide elections all the way down to local ones. All we would need to do is create a dictionary and list and modify our string. In this case, I replaced county name with contest name. Then, we would need to tweak our if statement and loop to get contest name from the contest dictionary.

![Contest_Name](https://github.com/dwwatson1/Election_Analysis/blob/main/Resources/Contest_Name.PNG)

![Contest_Extract](https://github.com/dwwatson1/Election_Analysis/blob/main/Resources/Contest_Extract.PNG)

![Contest_List](https://github.com/dwwatson1/Election_Analysis/blob/main/Resources/Contest_List.PNG)

## Project Difficulties
I had trouble completing git commits using GitBash. However, in realizing my initial error, I learn more about GitBash and a command lines than I would have had I not made this error. My initial error was naming my election analysis project __/Election-Analysis__ rather than __/Election_Analysis__. This caused an error in GitBash. I tried to rectify the error by renaming it to __/Election_Analysis__ and merging the data from __/Election-Analysis__. I ended up going down a deeper hole that I felt might erase all my work. I learned a lot from this experience (thanks for the tips Zeb!) and am confident I can nail this task in future projects.  
