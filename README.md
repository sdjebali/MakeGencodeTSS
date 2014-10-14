MakeGencodeTSS
==============

Makes distinct TSS of each gene from a Gencode annotation in GTF format

This script takes as input:
- a Gencode annotation file in GTF format (mandatory)
- a list of transcript biotypes to consider in this file (optional, default: no filtering)

This script provides as output the following files in the directory where it is executed:
- a file of most 5' exons from each transcript in GFF2 format
- a file of TSS from each transcript in GFF2 format
- a file of distinct TSS from each gene in GFF2 format, associated to a low confidence level in case the cds_start_NF 
  tag was present in any transcript with this TSS
