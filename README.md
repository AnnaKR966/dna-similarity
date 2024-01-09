# DNA similarity project
Project for SWBio data science course 

My SWBio rotation project is concerned with exploring the diversity within a collection of bacteriophages (phages), which are viruses that infect bacteria. A key element of this is how much the genomes differ between phages. Towards this end, the script is designed to compare all the possible combinations of phages and identify the number of matching bases. The majority of the genomes are around 60,000 kb, therefore this script acts as a prototype, to be scaled up to cover the 80 viral genomes with only modest changes to the input system.

The script has four major elements, it takes DNA sequences, finds the optimum alignment of two of them, calculates the percentage of identical bases, finally, once all the possible pairs have been compared it visualises all the data in an easy to read heatmap.

To run, download the jupyter notebook file entitled sequence_similarity.ipynb, which contains all the data required to run the script. The required packages are Biopython, Pandas and Seaborn.

The test DNA is embedded in the script, this loads the data into a dictionary, as a place holder for the individual importing the fasta files as SeqRecords directly into the nested for loop. The two part dictionary represents the record.id and record.seq of the SeqRecords. 

The nested loop ensures every combination of sequences is run through the alignment function. 

The percent function creates an optimal alignment and percentage of identical bases within that alignment. 

The output of the function records the compared sequences and percentage identity into a second dictionary. This second dictionary is then converted into a pandas dataframe and visualised as a heatmap.

The final part of the script is the exporting of the pandas dataframe and heatmap of the percentage identity between all the phages.

This pipeline allows for the easy comparison of how genetically identical the bacteriophages are by exporting, both a table showing the percentage identity between each pair of phages, and a graphical representation of it. 
