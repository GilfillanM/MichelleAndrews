# MichelleAndrews
### Hudson and Thames: A Machine Learning based Pairs Trading Investment Strategy

## Skill Set Challenge
Build a pairs selection framework to enable traders to build mean reverting strategies.
- Paper: Enhancing a Pairs Trading strategy with the application of Machine Learning
- Authors: Simão Moraes Sarmento and Nuno Horta

## Requirements and install
- yfinance
- pandas
- plotly.express
- sklearn
- numpy
- arch
- statsmodels

## Way of working

- I expored the problem statement by summarising all three components of Section III
- I tried to download data with different strategies even Wikipedia until I found a function that was simple enough to easily modify the time frame of stocks
- I applied PCA by viewing the time series as features and the stocks as observations.
- I researched different graphs to apply the OPTICS clustering to the PCA variables and discovered a 3Drotating graph.
- The pairs selection criteria needed further study therefore I read the book that was suggested on pairs trading strategies.
- I realized that each pairs selection criteria needed to be tested on each combination of pairs in each cluster
- I created a table to allow the trader to easily visualize each of the pairs selection criteria
- I finalized my report with PEP8 code style checks

## Design choices

- I choose plotly for 3D rotating graphs to visualize the clusters

## Learnings

- Trading pairs are difficult to visualize within high dimentional data sets like time series data over a long period of time. This experiment proposed a simple way to reduce the dimentionality of each availible stock with PCA. OPTICS clustering simplified this process even further by dividing the stocks into classes from which pairs could be chosen. I found it difficult to keep the pairs selection crteria function short as I wanted to eliminate as many unsuitable pairs as possible by implementing all the criteria for each possiblel pair within a cluster.
