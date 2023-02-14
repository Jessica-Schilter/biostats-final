# biostats-final
The datasets in these projects are all in the DATA folder

Instructions remain the same as for the midterm. 
Extra points (10% of total) for any insights outside of the questions asked.
Please use a notebook to submit code with comments, but also submit a
separate document with the answers. 

Two of these datasets you have already analyzed for the midterm. There is a new
dataset ppg2008.csv which is also used in lesson 11.

===========
Project 1.
===========
This data is about basketball players from the year 2008 and is
in the file ppg2008.csv. It has various statistics on players in the NBA.
You might not know what each of the metrics means (I don't),
but they are just different dimensions of data.  

This is a visualization and data mining exercise. 

What can you say about this dataset, use tools that you learned here.
and make a report or a visual that highlights something interesting,
maybe compare players, especially how they have performed since,
based on the data in here. Many of these players have reached
their peak recently and you will be able to find statistics about
their performance in 2019. 

Could you have predicted the successes and failures of some of the players, based
on analyses of the data ?
maybe you could be a talent scout for an NBA team ? 


Think of it as your job, as a reporter for NY times, to make a single graphic
that highlights something about this data. Explain the analysis that went
into the graphic and present the code too. This should be done in a notebook so
it is easy to evaluate. 



===========
Project 2.
===========

Dataset 2:  train.csv.gz
This is hand-written digits (0-9) from many people.
It contains 785 columns, first columns is digit and the 784 remaining columns
  are pixels 0-783. These are essentially 28x28 squares, so you can map the 784
  columns to entries in the squares. Each entry is 0-255, 0 is for black and 255
  stands for white, numbers in between are shades of gray


1) Use PCA to reduce dimensions.  How many components do you need to keep
to reproduce the digits reasonably well ? what is your final matrix ?

2) Draw a tree of the pixels, and see if you can explain the results based on
geometry of the pixels (how far apart are they in the 2-d space).
Try to Explain the PCA results in light of this. 

3) Can you use some of the tools you have learnt to build a classifier,
so if you get a new set of pixels you can predict what is in the
picture. This is a the start of a real project, but you don't have all the tools
 (such as neural networks) which might be more suited for this task.
Split your dataset into two (a training set and a test set),
build your classifier and figure out
how well it does with the test data in predicting the digits. 
Define the sensitivity and specificity of your classifier.
How well does it recognize your own handwriting
(make sure your handwriting is not in the training set)

4) You can try simple things like take average of all data for each number and
then take a "dot" product with your test set, and identify the pixels. This might
work, maybe for some digits, and not others.




===========
Project 3.
===========


Dataset 3: a) Mnemiopsis_col_data.csv b) Mnemiopsis_count_data.csv

This is gene expression data,  The columns represent samples, whose information is
in the col_data file. The count_data file contains counts for each gene (rows).
The file, info_gene.txt contains information about the organism and some links to
look up gene functions.
It will be a good experience to learn to use the genome resources,
as this is the kind of struggles most researchers go through when
they start looking at genes.


1) Build hierarchical trees based on the columns and for the rows (exclude rows
that are "low" expression)

2) Draw a heat map of the expression data

3) Use DESeq2 to analyse this data
   a) which are the most significantly changing genes in this dataset ?
   b) which genes are most consistently highly expressed in these datasets
       they are the "house-keeping" genes
   c) How consistent are these results with the analysis you did
      in the midterm project ? 
   d) What else can you say about the data in terms of consistency,
   and the results that you find from your analyses. The question is open-ended,
   think of this as your experiment, you need to write a paper based on this data
   so you have to figure out what kind of "story" you can tell based on this.
   
 e) what is the most interesting pathway or gene that is responding in this study?
   
 



