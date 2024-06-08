# Problem Statement  
Atliq media is a private media company and they wanted to telecast a show on Lok Sabha election 2024 in India. Unlike other channels they do not want to have a debate on who is going to win the election, they rather wanted to present insights from 2014 and 2019 elections without any bias and discuss less explored themes like voter turnout percentage in India.  

## 1. ASK  
Stakeholder: Bruce Haryali (Atliq CEO)  

### Questions:  
* List top 5/ bottom 5 constituencies of 2014 and 2019 in terms of voter turnout ratio?
* List top 5/ bottom 5 states of 2014 and 2019 in terms of voter turnout ratio?
* Which consistuencies have elected the same party for two consecutive elections, rank them by %votes to that winning party in 2019?
* Which consistuencies have voted for different parties in two election (list top 10 based on difference (2019-2014) in winner vote percentage in two elections.)
* Top 5 candidates based on margin difference with runners in 2014 and 2019?
* %Split of voters of parties between 2014 vs 2019 at national level.
* %Split of voters of parties between 2014 vs 2019 at state level.
* List top 5 constituencies for two major national parties where they have gained vote share in 2019 as compared to 2014?
* List top 5 constituencies for two major national parties where they have lost vote share in 2019 as compared to 2014?
* Which constituency has voted the most for NOTA?
* Which constituencies have elected candidates whose party has less than 10% vote share at state level in 2019?  

Further analysis & recommendations (Require additional research use secondary data)
* Is there a correlation between postal votes% and voter turnout% ?
* Is there a correlation between GDP votes% and voter turnout% ?
* Is there any correlation between literacy% of a state and voter turnout% ?
* Provide 3 recommendations on what the election commission/ goverment can do to increase the voter turnout% ?  

## 2. PREPARE  
### Data Storage:  
The public dataset is completely available on the Code basis website platform where it stores and consolidates all available datasets for analysis. The specific individual datasets at hand can be obtained at this link below: https://codebasics.io/challenge/codebasics-resume-project-challenge


### Data Organized:  
The dataset is taken from the Election Commission of India. Thanks to the ECI for providing datasets for public access which is a great learning asset - feel free to explore them here. https://www.eci.gov.in/statistical-reports  
This dataset contains only 3 csv file. 

## 3. PROCESS  

### Tools Used:  
* Microsoft Excel  
* Power BI  

### Data Used:  
dim_states_codes  
constituency_wise_results_2014, constituency_wise_results_2019  

### About Data:  
state: The name of the state where the election is held. This indicates the geographical location within India where the electoral process takes place.
dim_states_codes:  
- state_name: This column contains the full official names of states and union territories in India.  
- abbreviation:  The abbreviation column lists the standard two-letter codes assigned to each state and union territory.

constituency_wise_results_2014:
- pc_name: pc_name also knows as "Parliamentary Constituency Name". This column identifies the specific electoral district within the state from which representatives are elected to the Lok Sabha.  
- candidate: The name of the individual running for election. This is the person who is contesting in the election to become a Member of Parliament (MP).  
- sex: The gender of the candidate. Typically denoted as 'M' for male and 'F' for female.  
- age: The age of the candidate at the time of the election. This is given in full years.
- category: Refers to the reserved status of the candidate under Indian affirmative action policies, such as Scheduled Castes (SC), Scheduled Tribes (ST), or unreserved/general.
- party: The name of the political party that the candidate represents. If the candidate is not affiliated with any party, they are listed as an independent (IND).
- party_symbol: A unique symbol or logo assigned to the political party, which appears on the ballot paper. Independent candidates may have unique symbols that are not associated with a recognized party.
- general_votes: The number of votes the candidate received during the general voting phase. This does not include postal votes.
- postal_votes: The number of votes the candidate received via postal voting, which is typically used by voters who are unable to present themselves at the polling station on the day of the election.
- total_votes: The total number of votes received by the candidate, which is the sum of general votes and postal votes.
- total_electors: The total number of registered voters in the constituency. This gives an idea of the electoral size and the potential voter base from which the candidate can draw support.

state: The name of the state where the election is held. This indicates the geographical location within India where the electoral process takes place.


### Data Cleaning & Transformation:  
Microsoft Excel was used to clean and transform raw data.




## 4. ANALYZE  
### Key Metrics:  
* Voter Turnout Ratio: This metric represents the percentage of registered voters who actually cast their votes in an election. It is calculated by dividing the total number of votes cast (general votes plus postal votes) by the total number of registered electors in a constituency, and then multiplying by 100 to convert it into a percentage. This ratio is a crucial indicator of voter engagement and participation in the democratic process.  
Voter Turnout Ratio = (Total Votes Cast / Total Electors)× 100%


6. SHARE
7. ACT
