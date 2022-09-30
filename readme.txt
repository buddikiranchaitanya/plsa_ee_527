Included files:
-214161002_ML_Project_PLSA.ipynb: code file
-214161002_ML_Project_Report.pdf: project report
-data folder: contains the datasets
-readme.txt
-plots folder: images of plots used in the report

requirements:
numpy: 1.21.6
matplotlib: 3.2.2
pandas: 1.3.5
python: 3.7.13
tabulate: 0.8.9
random & math modules of python
-its assumed that dataset files are in a folder named 'data' and 
-the 'data' folder and ipynb file are in the same folder

The main code has been evaluated on 3 different datasets: KOS blog entries, NIPS papers &NYT articles.
For aesthetic purposes, I would prefer the NYT corpus, as it has diverse articles thus producing diverse & distinct topic.
There entire project is on a single ipynb file.

Procedure for running the code:
-run the blocks related to libraries and utility functions
-go to the blocks corresponding to the corpus you desire
-the first block under each corpus fetches the term document matrix 
-the second block runs the EM algorithm on the corpus, max iterations, number of topics & epsilon are hyper-parameters
-it takes around a minute for each iteration, thus, for mere code verification purpose it is suggested to use a small iteration number (<10)
-the existing results/outputs in the ipynb file correspond to outputs for 50-70 iterations run on google collar
-after the EM algorithm has ended, run the block below it to see the trajectory of Log Likelihood value vs iterations
-the final block displays the topics, with top-w (a parameter) words with highest probability being fetched from each topic



