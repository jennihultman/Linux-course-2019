# Problems

### NOTE: web-based tools are not allowed; everything should be performed in command line

### Please answer to the questions by writing the commands you used and explain their use

## Problem 1 
### (a)
**total 10 points**
Download from * [ftp NCBI server] (ftp://ftp.ncbi.nlm.nih.gov/genomes/genbank/bacteria/) directly on your CSC working directory from 50 randomly selected files of *Campylobacter jejuni* (nucleotide sequences of the CDS annotated for the selected genome) using the following format **cds_from_genomic.fna.gz**

and performed the following actions:

### (b) 
**total 10 points**
calculate the average number of CDS of the 50 samples

### (c)
**total 10 points**
delete all the CDS with length < 100 amino acid

### (d)
**total 10 points**
print in a new file the list of each *cds_from_genomic.fna* as results in point **(b)** including the complete path 
for example 

```
/wrk/mirossi/Linuxcourse/CjejuniCDS/ GCA_000254735.2_ASM25473v2.cds_from_genomic.fna
```

### (e)
**total 10 points**
From all the 50 samples as in point **(b)** extract in a single multifasta file the best blast hit (one for each sample; meaning the final file should contain a total of 50 fasta nucleotide sequence) for the ”multidrug efflux system gene” *cmeC* Cj0365c of the reference strain *C. jejuni* NCTC 11168 (you can download it e.g. from uniprotKB) and change the name of the headers of each fasta in the multifasta file to be sure that each entry header contains only the Genome accession number of the selected genomes (e.g. GCA_000254715.2 is the accession number of the file ’GCA_000254715.2_ASM25471v2_cds_from_genomic.fna.gz’)

### (f)
**total 10 points**
From the blast results as in point **(d)** extract for the best hit identity value and the score; make a single list with the extracted results in order from the highest score to the lowest

## Problem 2

### (a)
**total 10 points**
Download directly on your CSC working directory the draft genomes (contigs) of 10 *Campylobacter jejuni* genomes and 10 *Campylobacter coli* genomes (**genomic.fna.gz**) randomly selected from [ftp NCBI server] (ftp://ftp.ncbi.nlm.nih.gov/genomes/genbank/bacteria/)

### (b) 
**total 10 points**
Change the header of the contings in each genome as consecutive number 
e.g. for the genome GCA_000254735.2_ASM25473v2_genomic.fna.gz the list of the contigs headers are 

```
>AIOW01000129.1 Campylobacter jejuni subsp. jejuni 1997-4 n_202_l_199_c_20.658291, whole genome shotgun sequence
>AIOW01000128.1 Campylobacter jejuni subsp. jejuni 1997-4 n_179_l_209_c_39.540668, whole genome shotgun sequence
...
```

and they should be transformed as 

```
>1
>2
...
```

### (c) 
**total 10 points**
Calculate the frequency of presence of stretch of 9, 10 and 11 of single Cytosine (C) and Guanine (G) (e.g. GGGGGGGGG or CCCCCCCCC) in each genome a make a report
