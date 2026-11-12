# Project-1-Sequence-Analysis
Project DNA analysis that will sequence the DNA. 

Title and Purpose 

This project will use Pyhton to analyse the next generation sequencing (NSG) data from Schizosaccharomyces pombe investigating whether exposure to a genotoxic agent affects DNA mismatch frequencies compared with untreated controls.

How to Run the Program

The program is designed to run in Google Colab. One must open the project notebook , download required reference and sequencing data files using the provided cells and execute the analysis cells sequentially. 

Inputs and Outputs

The program will use a DNA reference sequence (reference.txt) and sequencing reads (reads.csv) from 6 biological samples that include 3 treated and 3 untreated controls. Each read is checked for validity before idetifying mismatches against the reference sequence. The analysis produces mutation information , sample level summarises and statisical comparisons of mismatch frequencies between the experimental groups. 

Code Design

The way I set up my program I tried to organise the program into seperate functions for validating DNA reads , analysing mutations , summarising samples and comparing mismatch positions. This allowed each function to perform a specific task and reduced repetition throught the analysis.

I used dictionaries to store information about individual reads and samples, including mutation counts, positions and mismatch percentages. This made it easier to access and organise results without creating too many separate variables.

I also included checks for invalid reads before analysing mutations to prevent incorrect sequences from affecting the results. Samples with no valid reads were handled separately to avoid the division by zero.
I chose these methods instead of writing a long function as the smaller functions for me were easier to test and correct when any error messages came up.

Testing

I tested the program using sample data sets and additional test cases that were given in the notebook. I , firstly , would check if valid and invalid DNA reads were correctly identified. Secondly I test sample summary function using an empty list to ensure it returned an empty dictionary. Finally I tested the position comparison function to check the mismatch percentages and statistical results were calculated correctly.
