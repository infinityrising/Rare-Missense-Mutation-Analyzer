# Rare Missense Mutation Analyzer

This python algorithm is designed to identify positional amino acid variants that are unusually rare for a particular sequence population (e.g., 10,000 sequenced HIV-1 Nef alleles). The algorithm takes an input amino acid alignment (.fasta) and analyzes each position for the particular amino acids that are present and the frequency of that amino acid among all the sequences. A cutoff can then be set to 1) identify any sequences with at least one missense mutations found at less than that given frequency, 2) identify the positions where these missense mutations are found, and 3) identify the amino acid that is rare. This program will also tell you the distribution of the other amino acids found at these positions. The data is output into table format in an excel workbook with 3 spreadsheets.

Example:

Take an input alignment of 500 HIV-1 Nef sequences. This program will look at each sequence, declare what the amino acid is in each position of that sequence, and tell you how frequently found that amino acid is found at that position across all the proteins in the alignment. If 10 out of 100 sequences have an "A" at position 2, then the "A" has a 10% frequency.

EXCEL WORKBOOK FORMAT

Spreadsheet 1: provides an output table that shows "% Frequency, Amino Acid, Aligned Position, Fasta ID"

Spreadsheet 2: provides an output table that shows "Fasta ID, Number of rare mutations"

Spreadsheet 3: provides an output table that shows "Number of rare polymorphisms, Number of sequences"

The third spreadsheet allows a better understanding of how unusual it is for a particular protein to have a particular number of rare polymorphisms.

I hope that you find this tool useful for your research.

Zacko
