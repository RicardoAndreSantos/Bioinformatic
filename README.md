# Bioinformatic
Work developed for bioinformatic course

### Assignment_1
Alignment of nucleotide (i.e., genes) or amino acid (i.e., proteins) pairs of sequences allows determining the similarity between two sequences.
Alignments between pairs of phylogenetically close sequences usually result in optimal complete alignments.
For the global alignment, it was used the algorithm developed by Needleman and Wunsch.
In the local alignments the algorithms developed by Smith and Waterman seek to maximize the best alignment between subsequences.

#### objectives:
* implementation of global and local alignment through dynamic programming;
* use of a REST web service to remotely test the algorithms developed (i.e., global and local alignment in gene and protein databases such as European Nucleotide Archived (ENA) and UniProt).

---

### Assignment_2
Identification of coding and non-coding regions: Hidden Markov Models. </br>
The Viterbi algorithm will return the most likely path to generate a given sequence. </br>
The Forward algorithm will tell us the probability of a particular sequence.

#### objectives:
* implementation of a hidden Markov model to predict coding regions (genes present in DNA sequences);
* Viterbi and Forward algorithms.

---

### Assignment_3
Implementation of Phylogenetic Trees. </br>
Phylogenetic trees translate the relationships between sequences (genes or proteins) as well as species. </br>
The unweighted pair group method with arithmetic (UPGMA) is a simple agglomerative hierarchical clustering method that starts from an array of distances to find the least divergent pair of sequences. </br>
The distances are then recalculated relative to the new cluster. This process is repeated successively until all the sequences are hierarchically grouped to a single node or root.

#### objectives:
* implementation of the UPGMA algorithm;
* compare the UPGMA algorithm with other phylogenetic methods (Phyllip).
