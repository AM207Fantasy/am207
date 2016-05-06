# AM 207 Final Project: Stochastic Methods for Fantasy Basketball

Final project for Harvard's Applied Math 207: Stochastic Methods for
Data Analysis, Inference, and Optimization, Spring 2016.

By: Xingchi Dai, Andy Shi, Hyungmok Son, Hidenori Tanaka

---

Check out our [report](https://github.com/AM207Fantasy/am207/blob/master/AM207_Final_Project_Report.pdf)
and [poster](https://github.com/AM207Fantasy/am207/blob/master/AM207_Poster.pdf)!

Link to our screencast: https://youtu.be/zmZmO3sPxx8

## Description of Files

### Data

The raw data, in the form of CSV files, are all stored in the in the
`raw-data` folder.  See the README in there for more information. After
the data gets cleaned, the cleaned data are stored in the `clean-data`
folder.

### Data Cleaning

+ `data-cleaning.ipynb`: This file contains code to convert the raw data
  into a form more amenable for analysis. Here, we merge information
  about players' salary and their game statistics, remove NaN values,
  and create matrices that we will need for indexing purposes.

### Lineup Selection

+ `Simulated Annealing .ipynb`: This file contains code for the
  simulated annealing and the greedy algorithm, which were used to pick
  the best lineup.

### Player Contribution Estimation

The notebooks that address this are the following (you should read them
in this order):

+ `lbfgs-sgd.ipynb`: Contains code for L-BFGS and SGD.
+ `Pymc and Pooling.ipynb`: Contains code for our first implementation
  of PyMC
+ `Cluster and optimize.ipynb`: Contains implementation of clustering
  with PyMC.
+ `ESS_a single game.ipynb`: Contains code for running elliptical slice
  sampling (ESS) on a single game.
+ `ESS_entire games.ipynb`: Contains code for running ESS on the whole
  season.
+ `Simulated Annealing.ipynb`: Contains code for running simulated annealing to find the best line-up basketball team
+ `pystan.ipynb`: Contains code for a model in PyStan.

### Player Condition

This is implemented in the notebook `Condition Estimation.ipynb`.

### Other Folders

+ `attic`: Contains old stuff we didn't actually use
+ `figure`: Just an empty folder---running the code will put figures
  here
