# DNA similarity project
Project for SWBio data science course 

My SWBio rotation project is concerned with exploring the diversity within a collection of bacteriophages, which are viruses that infect bacteria. The majority of the genomes are around 60,000 kb.

Towards this end, the script is designed to take DNA sequences, find the optimum alignment, and output the percentage of identical bases into an easy to read heatmap. This has been designed as proto type to be scaled up to cover the 80 viral genomes with only modest changes to the input system.


To run, download the jupyter noteook file entitled sequence_similarity.ipynb, which contains all the data required to run the script. The required packages are Biopython, Pandas and Seaborn.

The test DNA is embedded  in the script, this loads the data into a dictionary as a place holder for the individual importing the fasta files as SeqRecords directly into the nested for loop. The two part dictionary represents the record.id and record.seq of the SeqRecords. 

The nested loop ensures every combination of sequences is run through the alignment function. 

This function creates an optimal alignment and percentage of identical bases within that alignment. 

The output of the function records the compared sequences and percentage identity into a second dictionary. This second dictionary is then converted into a pandas dataframe and visualised as a heatmap.

This pipeline allows the for the easy comparison of the how genetically identical the bacteriophages are by exporting, both a table showing the percentage identity between each pair of phages, and a graphical representation of it. 
