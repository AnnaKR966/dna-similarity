# DNA similarity project
Project for SWBio data science course 

My SWBio rotation project is concerned with exploring the diveristy within a collection of bacteriophages, which are viruses that infect bacteria. The majority of the genomes are around 60,000 kb.

Towards this end, the script is designed to take DNA sequences, find the optimium alignment, and output the pecentage of identical bases into an easy to read heatmap. This has been designed as proto type to be scaled up to cover the 80 viral genomes with only modst changes to the input system.

The test DNA is embeded in the script, this loads the data into a dictionary as a place holder for indivdualling importing SeqRecords directly into the nested loop. The nested loop ensures every combination of sequences is run through the alignment function. This function creates an optimal alignment and percentage of identical bases within that alignment. The output of the function records the compared sequences and percentage identity into a second dictionary. This second dictionary is then converted into a pandas dataframe and visualised as a heatmap.

The required packages are Biopython, Pandas and Seaborn.
