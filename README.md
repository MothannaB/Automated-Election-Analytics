# Automated Election Analytics & Reporting Pipeline

This Python application automates the process of analyzing election results. It reads a raw CSV data file containing ballot information, calculates key election metrics, and outputs a formatted report to both the terminal and a text file.

---

## Features

* **Total Vote Calculation:** Counts the total number of votes cast in the election.
* **County-Level Analysis:** Calculates the total votes and percentage of turnout for each county.
* **Turnout Leader:** Identifies the county with the largest voter turnout.
* **Candidate Standings:** Calculates the total votes and percentage of votes won by each candidate.
* **Winner Determination:** Determines the winning candidate based on the popular vote.
* **Dual Output:** Outputs results directly to the terminal and automatically writes them to an audit-ready text file.

---

## File Structure

```text
automated-election-pipeline/
│
├── Resources/
│   └── election_results.csv        # Raw input dataset (ballot logs)
│
├── analysis/
│   └── election_analysis.txt       # Generated output report
│
└── election_analysis.py            # Core Python script

```
Sample Output Report
Once executed, the application generates a report that looks like this:

Election Results
-------------------------
Total Votes: 369,711
-------------------------

County Votes:
Jefferson: 10.5% (38,855)
Denver: 82.8% (306,055)
Arapahoe: 6.7% (24,801)

-------------------------
Largest County Turnout: Denver
-------------------------
Charles Casper Stockham: 23.0% (85,213)
Diana DeGette: 73.8% (272,890)
Raymon Anthony Doane: 3.1% (11,606)

-------------------------
Winner: Diana DeGette
Winning Vote Count: 272,890
Winning Percentage: 73.8%
-------------------------
