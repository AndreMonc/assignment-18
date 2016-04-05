# Task 1

In `task1-files`, there is a text file of different species names.  Write a general program that takes this list as input (using `argparse`) and gets the taxonomic information from NCBI for each samples and writes that to a new file as output (again, get the output file name using `argparse`).  Format the output file as a CSV.  The output file should contain the values for each species for the following: `superclass, class, subclass, infraclass, superorder, order, superfamily, family, and genus`.  Be sure that your program is formatted correctly (`PEP8`) and be sure that your file works appropriately with any generic list of species. Also be sure that you pass your name to NCBI (`Entrez.email`) and that you limit your requests to 1 per second.

# Task 2

_Loxosceles reclusa_ is also known as the "brown recluse", a spider that is known to occasionally bite humans and the bites of which cause severe tissue necrosis around the site of the bite.  Write a program that queries GenBank for all the sequence data for this spider and then writes the sequence data to a file in FASTA format.  Use `argparse` to take the name of the organism as input and the name of some FASTA file as output. Be sure that your program is formatted correctly (`PEP8`). Also be sure that you pass your name to NCBI (`Entrez.email`) and that you limit your requests to 1 per second.

# Task 3

Building on `Task 2`, modify your program above to get GI record of each sequence from NCBI (e.g. do not work from the FASTA file you created) and the send those records to NCBI BLAST to perform a `blastn` search of each sequence against the `nt` (nucleotide) database.  Write each BLAST result (the result for each sequence, which may consist of several hits) out to text files in BLAST format (use `argparse` to get the output directory name from the user).  We didn't cover BLAST searches in class, so you'll need to look at the [BioPython Cookbook](http://biopython.org/DIST/docs/tutorial/Tutorial.html#htoc86) and go from there. Be sure that your program is formatted correctly (`PEP8`). Also be sure that you pass your name to NCBI (`Entrez.email`) and that you limit your requests to 1 per second.
