# Homework 6: ****DRAFT**** 

**NOTE: This is not the actual assignment yet!**
We will begin analysis of two actual datasets from a human vaginal microbiome study. 

In this assignment we will read in two actual empirical datasets, combine the data, and do some simple data processing. 

***describe the datasets, cite PNAS, describe reason for study***
### Readings
1. Read and meditate upon *The Zen of Python*, [https://en.wikipedia.org/wiki/Zen_of_Python](https://en.wikipedia.org/wiki/Zen_of_Python)
2. Read [https://www.python.org/dev/peps/pep-0008/](https://www.python.org/dev/peps/pep-0008/)
2. Work through [https://docs.python.org/3.5/tutorial/errors.html](https://docs.python.org/3.5/tutorial/errors.html)
3. Work through textbook, Chapter 5, *Getting Started with Pandas*, pages 107--132
## Things to do before beginning of class, **DATE (Lecture XXX)**, or sooner
Write a program named *microbiome.py* that does the following:

1. Read *../Resources/vaginal_communities.txt* into an appropriate data structure. 

	Later you will want to group the data by patientID and timepoint (which is derived from week and day), and you will display data for each microbial group. 

	a. In your comments, justify your choice of this data structure, so the next programmer knows **why** you did it this way.

2. Change all OTU counts to relative abundances (the relative abundance is the read counts--the number in columns--divided by the total count in *Total*)

	OTUs are Operational Taxonomic Units, groups of similar sequences which are named by looking up those sequences in an existing database. Sometimes this is a species name, sometimes it is not.
3. Compute the average relative abundance of each OTU for each patient.

	a. Be sure to handle errors (there are likely to be some, since this is real-world data)
4. Write a tab delimited file named *avgRelativeAbundances.txt* that has the patient ID and the average relative abundances for each OTU.

	a. Sort the records by the patient ID
	b. Keep the columns in the same relative order as in the input file
	b. Retain the column headers from the input file. (we will use this file in later assignments)
## Turn in homework

1. Commit your work
2. Update your local master
3. Sync with the remote master

## Grading
Grades will be determined as follows:

Grade | Criteria 
-------- | --------------
0          | Nothing turned in
1          | Code turned in but doesn't run, or is incorrect
2          | *avgRelativeAbundances.txt* is correct
3          | *avgRelativeAbundances.txt* is correct, and code uses good style (as per our readings on style)