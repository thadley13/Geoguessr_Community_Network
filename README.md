# Geoguessr_Community_Network
Includes network data that describes the connections between members of a community of professional Geoguessr players.

Description: \n
The professional Geoguessr player Rainbolt would hold weekly tournaments where teams competed against each other. The selection of teams is assumed to be governed by the social interactions within the community. A network of 'teammate connections' can be made to study the social dynamics within the community and how they evolve. In this context, nodes are participants in these tournaments, and edges exist between nodes if they were on the same team for a given tournament.

Node Metadata:
Num_Wins: to date

Edge Metadata:
Score: Provides a measurement of performance of the team of this node for a given tournament. The range of scores is between 0 and 100. Score calculated as 100 - 100*(Position / Num_Teams). Position reflects the position a team finished in a given tournament. Note there are often many ties between teams, and positions are calculated as the average of the range of positions where there is a tie. For example, for a semifinalist, the position recorded is 3.5, and for a quarterfinalist, the position recorded is 6.5 Num_Teams represents the number of teams competing in this tournament.
Win: A binary variable that tracks whether a connection is part of a winning team.
Date: The Date for which the connection takes place.

Basic Network Stats:
Nodes: 207
Edges: 1992
**Note** The same edge may exist several times in the data, but a different dates, representing a different tournament.

Applications:
This data is sufficient for constructing temporal network analyses to track online community development and growth for this particular case. The date metadata allows for the construction of several sub-networks, at different time intervals.
This data is perfect for analysis on the effect of skill/success on the popularity of individuals in an online community.

Privacy:
The usernames of participants are hidden in this dataset, and nodes are labelled by number only.

Source: 
This data was taken from weekly tournaments, hosted by Geoguessr player Rainbolt. Recordings of these tournaments can be found here: https://www.youtube.com/@georainbolt/videos.
Tournament result data was collected from these videos, and scraped from the following Google Spreadsheet: https://docs.google.com/spreadsheets/d/1x-24IlfpIwWwe9vRQENsnAd5PHG6hl9EyTndY36iCFY/edit#gid=1500096509
