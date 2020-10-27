# GCF_variation_Bacillus
Analysis of the variation within Gene Cluster Family of Bacillus sp. 

This repository contains Jupyter Notebook describing a workflow for analyzing variations within a Gene Cluster Family (GCF). The software tools that are used to generate the data include antiSMASH (to detect Biosynthetic Gene Clusters (BGCs)), BiGSCAPE (to detect GCFs), Cytoscape (to visualize the networks).

The repository requires users to define genome dataset, run antiSMASH and BiGSCAPE analysis independently. These steps and the output data is not included in this repository due to large size of the data. We expect the readers to be familiar with running the genome mining tools such as antiSMASH and BiGSCAPE. For further, information on these initial steps please contact the authors (omkmoh@biosustain.dtu.dk)

### Data directories used in this analysis

Following data directory structure was used to store the data and we recommend the users to follow similar data structure or adapt the notebooks accordingly.

    1. ../data/antismash_out : Output folders for all genomes in analysis also used as input for BiGSCAPE software. This is not included in the Github directory, and users can adapt this locally. We use this data only to extract amino acid specificity in this analysis, which part should be adapted accordingly.
    2. ../data/bigscape : Output of BiGSCAPE dataset, which will be used to create network and detect families
    3. ../data/cytoscape : To save tables to be used by Cytoscape for visualization
    4. ../data/bigscape_selected : Rerunning BiGSCAPE for subgroups within specific GCFs to generate CORASSON alignments
    5. ../data/frameshift : Nucleotide sequence alignments for selected genes to show conserved frameshift mutations
    6. ../tables : Directory to save tables with information on BGCs  
