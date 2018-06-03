Exercise 1: downloading and using publicly available NGS data

In recent years, a huge amount of NGS experiments have been conducted in a wide variety of organisms. When these studies are published, the raw sequence reads should be made publicly available and are often deposited in the Sequence Read Archive (https://www.ncbi.nlm.nih.gov/sra). 
This means that there is a lot of data out there to be mined!

In this exercise we will be downloading and aligning sequencing data produced from a recent study from Jia et al, 2016 involving several different Maize mutant lines.
The aim of this exercise is to become familiar with publicly available NGS data, critically assessing the quality of your data, selecting suitable reference sequences, trying out different methods for sequence alignment and manipulating the output.

The steps below give an outline and suggestions for the work flow, but feel free to explore anything you think could be interesting at each step!

1. Download exome-seq FASTQ files for Mutants 146, 1554 and 1115 from Jia et al, 2016 (http://www.g3journal.org/content/6/8/2385)
    - Hint: Papers should include a data availability statement which will include SRA accession codes
    - Tip: European Nucleotide Archive (https://www.ebi.ac.uk/ena) has a more user friendly interface for downloading files directly from the webpage
		
2. While the files are downloading, make sure you understand the experimental design used to produce these reads.
    - What type of sequencing data is this? 
    - What platform was it produced with?
    - What Maize accession was used?
    - Any other important details?

3. Use FastQC to assess the quality of the FASTQ files you have downloaded.
    - How does the quality of the fastq files look?
    - Anything unexpected?
    - Do they require further processing before alignment?
    - How many reads in each file?
		
4. Trim the reads and reassess the quality.
	- What difference, if any, has the trimming process made?

5. Find and download an appropriate reference sequence that can be used for mapping reads.
	- Did you have multiple options for the reference sequence?
	- If so, what made you select this one?
	- Is it a 'good' reference sequence? Why/why not?
	- Is the genome assembled into chromosomes? How many? How large is the assembly?
	
6. Map both the trimmed reads to the reference, using the tool of your choice.

7. Create a table of summary statistics about the mapping outputs and plot some coverage statistics.
    - Hint: think about what statistics will be useful to use to assess quality e.g. % mapped reads, depth etc.

8. Map the untrimmed reads - how much did trimming the reads affect the quality of the mapping output?

9. Try mapping the reads using a few different mapping tools, which performs best in this case?

	** This could be done as a small group exercise - each person choose a different tool to experiment with and compare output at the end.**
	- HINT: You will probably need to search online and in the manuals to find out how to run the tools!
	
10. Additional things to explore:
    - Inspect your mapping outputs using a browser, such as IGV or Tablet.
    - Try also loading the genome annotation into the browser to see how the alignments relate to genes
    - Is the coverage distributed evenly across the genome? If not, why not?
    - Is the average coverage roughly what you would expect given the number of reads in the fastq files?
    - Try filtering your alignments for various parameters
    - In the paper, the authors are interested in the gene Sugary-1. Can you extract the alignments for just the region containing this gene?
    - Do all the alignments for Sugary-1 look the same in all 3 mutants? If not, what is different?
	
If you have time:

Try finding available NGS data for your own species of interest, find a reference and test out some alignments.
Choose a gene you are interested in...how do the alignments look across this gene?

	

	

