JASPARscraper.ipynb creates the database JASPAR_new.txt from a scraping of the vertebrate JASPAR site (http://jaspar.genereg.net/cgi-bin/jaspar_db.pl?rm=browse&db=core&tax_group=vertebrates).

CLOVER was obtained from http://cagt.bu.edu/page/Clover_about

The following was run from the command line:
clover -t 0.05 JASPAR_new.txt promsequences.fa > promresults.txt

CreatePSMMfromCLOVER.ipynb creates the position specific motif matrix (PSMM) (PSMM_5seg2.csv) from promresults.txt.  The variable “featurenames” is a list of the column-names.  The variable “genes” is a list of the row-names.

