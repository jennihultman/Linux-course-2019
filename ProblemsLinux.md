# Linux Problems

### NOTE: web-based tools are not allowed; everything should be performed in command line

### Please answer to the questions by writing the commands you used and explain their use

## Question 1
**Points: 5**

You will be using program that will need a file from your $WRKDIR directory to be in the same directory ($HOME) where you run the program. However, the file is 5 GB and does not fit to your $HOME. What can you do? 

## Question 2

You run a BLAST search against 16S rRNA gene database using the following command

```
pb blastn -dbnuc current_GREENGENES_gg16S_unaligned.fasta -query myseq.fastq -out blastoutput.txt -outfmt 6 -num_descriptions 1
```

please answer the following questions

## (a)
**Points: 2**

What do the used parameters mean? And what are the columns in the output?

## (b)
**Points: 8**

For further analysis you’ll need to modify the output. Write the results as a text file with
-	first column for the accession number 
-	second for the sorted number of hits to that accession number

## Question 3

## (a)
**Points: 2**

Open a new terminal window. Check from the first one in which taito node you are logged in to. In the new terminal log into the same node. Download all cds of a bacterial genome of your choice from [ftp NCBI server] (ftp://ftp.ncbi.nlm.nih.gov/genomes/genbank/bacteria/). 

## (b)
**Points: 3**

Modify the gene names removing *locustag*, *protein*, *protein_id*, *location* and *gbkey*. The new name should contain only

```
>lcl| accessionumber_cds_number 
```

## (c)
**Points: 5**

Calculate the number of genes and extract the 50 first genes into a new file. From the file with the 50 first genes check by eyeballing and highlighting if TTTTTTT is found and eventually count the frequency.

## Question 4 

### (a)
**Points: 1**

Download from * [ftp NCBI server] (ftp://ftp.ncbi.nlm.nih.gov/genomes/genbank/bacteria/) directly on your CSC working directory from 5 randomly selected files of *Campylobacter jejuni* (nucleotide sequences of the CDS annotated for the selected genome) using the following format **cds_from_genomic.fna.gz** and calculate the average number of CDS of the 5 samples.

### (b)
**Points: 4**

Print in a new file the list of each file you downloaded including the complete path. 
For example: 

```
/wrk/mirossi/Linuxcourse/CjejuniCDS/New_GCA_000254735.2_ASM25473v2.cds_from_genomic.fna
```

### (c)
**Points: 4**

Delete all the CDS with length < 100 amino acid from the 5 **cds_from_genomic.fna.gz** you dowloaded and save the results in a new file named *New_accession number.cds_from_genomic.fna*.

### (d)
**Points: 8**

From the 5 samples you downloaded extract in a single multifasta file the best blast hit (one for each sample; meaning the final file should contain a total of 50 fasta nucleotide sequence) for the ”multidrug efflux system gene” *cmeC* Cj0365c of the reference strain *C. jejuni* NCTC 11168 (you can download it e.g. from uniprotKB) and change the name of the headers of each fasta in the multifasta file to be sure that each entry header contains only the Genome accession number of the selected genomes (e.g. GCA_000254715.2 is the accession number of the file ’GCA_000254715.2_ASM25471v2_cds_from_genomic.fna.gz’)

### (e)
**Points: 8**

From the blast results as in point **(d)** extract for the best hit identity value and the score; make a single list with the extracted results in order from the highest score to the lowest

## Question 5
**Points: 10**

Download the draft genome (contigs) of GCA_000254735.2_ASM25473v2 from [ftp NCBI server] (ftp://ftp.ncbi.nlm.nih.gov/genomes/genbank/bacteria/) and change the header of the contings as consecutive number 
for example:

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

## Submit your essay to the teacher
Save your results as a *.txt* file and move them to a shared folder in your *wrk* directory. Make sure to give **Jenni** and **Mirko** access to your results (*look carefully the instructions on CSC webpage and remember to share the file with **all users***). Finally, send to us an Email with the path where is your essay in your CSC account. **Note: we will accept only essays which are on your CSC account. If the file is not accessible to us you will fail the exam.**

You will pass the exam with 45 out of 60 points.
We will consider also partial answers.

# Good luck!!!

