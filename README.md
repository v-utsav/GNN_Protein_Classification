In this project, I have built a GNN to classify proteins according to their functions.

Classifying proteins according to their functions is an important task in bioinformatics.
By classifying them, we can learn their function which helps to understand biologi-
cal processes and has practical applications such as medicine and pharmaceutical
research. Classification remains a challenging problem as there generally are no un-
ambiguous features - there is a lot of variety in the same class, and relatively similarly
structured proteins can have very different functions.
Proteins consist of polypeptides, which are long chains of amino acids - sometimes
several of these form a protein complex. There are 20 different amino acids that com-
monly appear as part of proteins. They can be represented by their ordered sequence,
but also fold in 3D space into a specific form, where their properties can be analyzed
as a graph. The amino acids are represented by the nodes and their 3D positions, and
edges are formed based on proximity, sequence order, and chemical interactions. 

Input files:
sequences.txt: Amino acids can be represented by their full name, a three letter code
or a one-letter-code, which we will use here. It assigns a letter of the alphabet to
each of the common amino acids. This file contains the amino acid sequences of
each protein represented by this code.

node attributes.txt: Each node has a 3D position in the first 3 entries, followed by a
variety of properties.

edgelist.txt: The existing edges between nodes.
edge attributes.txt: Each line contains the distance between the nodes, filled by bi-
nary indicators of the edge types based on distance, peptide bonds, k-nearest
neighbor, and hydrogen bonds.

graph indicator.txt: This file has a graph identification number in each line to assign
each node to its respective graph.

graph labels.txt: Here you can find the protein identifiers (4 letter code) and function
classes of the training set.
