# Project-1-Sequence-Analysis
Project DNA analysis that will sequence the DNA. 

Title and Purpose 

This project will use Pyhton to analyse the next generation sequencing (NSG) data from Schizosaccharomyces pombe investigating whether exposure to a genotoxic agent affects DNA mismatch frequencies compared with untreated controls.

How to Run the Program

The program is designed to run in Google Colab. One must open the project notebook , download required reference and sequencing data files using the provided cells and execute the analysis cells sequentially. 

Inputs and Outputs

The program will use a DNA reference sequence (reference.txt) and sequencing reads (reads.csv) from 6 biological samples that include 3 treated and 3 untreated controls. Each read is checked for validity before idetifying mismatches against the reference sequence. The analysis produces mutation information , sample level summarises and statisical comparisons of mismatch frequencies between the experimental groups. 

Code Design
