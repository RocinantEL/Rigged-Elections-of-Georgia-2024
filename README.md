# Rigged-Elections-of-Georgia-2024

(This repository contains a Python-based simulation for analyzing election data and detecting irregularities by comparing simulated election results to official outcomes. The project uses official "CEC" election data to simulate voting outcomes, apply Gaussian noise to the voting probabilities, and compare the simulated distribution to official results, allowing for the detection of potential election falsification.

This code simulates election outcomes using official "CEC" election data, applying Gaussian noise to simulate natural variations in voting behavior. The simulation results are then compared with the official distribution of votes for a particular political party. This approach can help identify discrepancies that may suggest potential electoral fraud.

Tructure of the code is the following:
Simulate Elections: Simulate vote distributions for a given party across multiple precincts using official vote percentage data.
Gaussian Perturbation: Apply random Gaussian noise to simulate natural fluctuations in voter behavior across precincts.
Comparison with Official Data: Compare the simulated election results to the official distribution of votes and visualize them as histograms.
Detection of Irregularities: Identify discrepancies between simulated and official distributions, which may suggest election falsification.

more details about the code:
Data Input: The script reads election data, including the total votes per precinct and the official percentages for different political parties.
Simulated Voting: The simulation assigns each precinct a probability for voting based on official data, perturbs these probabilities with Gaussian noise, and simulates voter choices.
Gaussian Noise: Apply Gaussian noise to reflect natural voting variability. Different levels of noise are tested to simulate more or less variation.
Comparison: Compare the results to the official vote distribution, and generate a histogram for visual analysis.
Visualization: Plot the results of each simulation run alongside the official results to visually assess any discrepancies.

The code requires:
Python 3.x or higher

pandas
matplotlib
numpy
scipy
random
collections)

(as you can see, here we present our project that proves the falsification of the elections 2024 in Georgia.
all the "CSV", "xlsx" and "pbx" files are data sets used in the codes except of the files "Election-Charts" and "Final-Source".)

•(Elections-Charts.pbix represents the visualization of the election 2024 results throughout whole Georgia.
The file shows how the Fig.1 chart in the paper was constructed using the official "CEC" data. In this file you can see the graphs of Precints’ frequency distribution by percents and political parties (that have passed the 5% electoral threshold) and take a look at how specific political party performed in different regions or demographically similar units, and compare the parties’ results to each other.
To be able to use the contents of the file you should first make sure to have installed the Microsoft Power BI Desktop on your device. If don’t have it already you can download it freely from:
https://www.microsoft.com/en-us/download/details.aspx?id=58494
•	Final-Source.xlsx represents the source data for Elections-Charts.pbix file. In this file you can see the official "CEC" data of election results and also some supporting sheets, including demographic stratifications and dimension tables for data model used in Elections-Charts.pbix.)


("Statistics of CESKO" file is a dataset of the turnouts and percentages of "The Georgian Dream Party", and this file is used for Density graph in tha paper (Fig.2)


"density" file is the code that constructs the Fig.2 in the paper


"election_size" is the dataset of the precincts and how many people voted in those precincts in total (used in the main code)


"electoraldistrictprb" file is an official percentage of each political party in each and every electoral district (used in the main code)


"realdist5%" is a dataset of the real official distribution for 5% bin size (used in a main code)


"1-BINS" is a dataset of the real official distribution for 1% bin size (used in a main code))
