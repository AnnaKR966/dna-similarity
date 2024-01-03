# DNA similarity project
Project for SWBio data science course 

Within my rotation project I am working with a collection of bacteriophages, which are viruses with DNA of around 60,000 kb. I am particularly concerned with ensuring diversity within the collection.  

Towards this end, the script is designed as proto type to be scaled up to cover the 80 viral genomes. 

Initially the script loads the data into a dictionary, from which a nested loop creates an optimal alignment and records the alignment score. This score is turned into a percentage of the similarity and recorded into a second dictionary. This second dictionary is then converted into a pandas dataframe and visualised as a heatmap.  

The required packages are Biopython, Pandas and Seaborn 
