# Applied Statistics - Problems <br /> 
<br /> 
Applied Statistics - Problems contains all the tasks/problems in the Higher Diploma in Data Analytics course for this module 
<br /> 
<br /> 
Here I will explain how I came to the solution of given problems, reference the sources I researched for solving the problems and list the technologies I used for creating and testing the code. <br />
<br />
<br />



https://github.com/binder-examples/requirements/blob/main/README.md

# Table of contents - Tasks
* [Software needed to run the tasks](#software-needed-to-run-the-tasks)	
* [Problems](#problems)   
    * [problem 1 Extending the Lady Tasting Tea](#problem-1-extending-the-lady-tasting-tea)
    * [problem 2 Normal Distribution](#problem-2-normal-distribution)
    * [problem3 t-Tests](#problem3-t-tests)
    * [problem4](#problem4)
    

Software needed to run the Tasks
======

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. The requirements.txt file should list all Python libraries that your notebooks depend on, and they will be installed using: <br />
pip install -r requirements.txt<br />
<br />
<br />

Please see below as an example of the main packages that I am using for the problems and analyses.

- Download Anaconda - Anaconda is a package that aims to simplify package management 
- Download Visual Studio Code
- Jupyer Notebook
- Download Github - https://github.com/AudeAllen/Applied_Statistics.git
- To run the problems simply click on 'Run all' for problems.ipynb. The project is a mix of code and markdown blocks which explain each part of each task. You can perform this action either in Visual Studio code or in Anconda in Jupyer Notebook.

Problems
======
### ***Problem 1 Extending the Lady Tasting Tea***

Let's extend the Lady Tasting Tea experiment as follows.
The original experiment has 8 cups: 4 tea-first and 4 milk-first.
Suppose we prepare 12 cups: 8 tea-first and 4 milk-first.
A participant claims they can tell which was poured first.  

Simulate this experiment using `numpy` by randomly shuffling the cups many times and calculating the probability of the participant correctly identifying all cups by chance.
Compare your result with the original 8-cup experiment.  

In your notebook, explain your simulation process clearly, report and interpret the estimated probability, and discuss whether, based on this probability, you would consider extending or relaxing the p-value threshold compared to the original design.  

References <br />

https://www.codecademy.com/resources/docs/python/math-module/math-comb <br />
https://numpy.org/doc/stable/reference/random/generated/numpy.random.seed.html <br />
https://docs.python.org/3/tutorial/introduction.html#lists <br />
https://realpython.com/monte-carlo-python/ <br />
https://realpython.com/for-loop-python/ <br />
https://numpy.org/doc/stable/reference/random/generated/numpy.random.permutation.html <br />
https://numpy.org/doc/stable/reference/generated/numpy.array_equal.html <br />
https://docs.python.org/3/library/string.html#format-specification-mini-language <br />
https://chatgpt.com/share/68f11265-8a68-8012-9b46-84dbe72c2aa5 <br />

======
### ***Problem 2 Normal Distribution***

Generate 100,000 samples of size 10 from the standard normal distribution. For each sample, compute the standard deviation with ddof=1 (sample SD) and with ddof=0 (population SD). Plot histograms of both sets of values on the same axes with transparency. Describe the differences you see. Explain how you expect these differences to change if the sample size is increased.

References <br />

https://www.datacamp.com/blog/standard-normal-distribution<br />
https://www.geeksforgeeks.org/python/python-normal-distribution-in-statistics/<br />
https://www.geeksforgeeks.org/python/numpy-std-in-python/<br />
https://medium.com/@bluewall_46049/standard-deviation-variance-2424395a13be<br />
https://chatgpt.com/share/691b6de7-a24c-8012-8b0c-677b600fa54b<br />

======
### ***Problem3 t-Tests***

A type II error occurs when a test fails to reject the null hypothesis even though it is false.
For each mean difference $d = 0, 0.1, 0.2, \dots, 1.0$, repeat the following simulation 1,000 times:

1. Draw two samples of size 100, one from the standard normal distribution and one from the normal distribution with mean $d$ and standard deviation 1.
2. Run an independent samples t-test on the two samples, rejecting the null hypothesis if the p-value is less than 0.05.
3. Record the proportion of times the null hypothesis is not rejected.

References <br />

https://www.scribbr.com/statistics/null-and-alternative-hypotheses/<br />
https://en.wikipedia.org/wiki/Type_I_and_type_II_errors<br />
https://projects.iq.harvard.edu/statistics/book/error-types<br />
https://www.optimizely.com/optimization-glossary/type-2-error/#:~:text=Type%20II%20errors%20are%20like,exist%20when%20it%20actually%20does<br />
https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.ttest_ind.html<br />
https://numpy.org/doc/stable/reference/random/generated/numpy.random.normal.html  <br />  
https://github.com/xaviervasques/t-test/blob/master/ttest_scipy.py <br />
https://matplotlib.org/stable/api/pyplot_api.html   <br />
https://docs.python.org/3/library/stdtypes.html#mapping-types-dict<br />
https://www.w3schools.com/python/python_dictionaries.asp <br />
https://www.pythoncheatsheet.org/cheatsheet/dictionaries<br />

======
### ***problem4 ANOVA***

Generate three independent samples, each of size 30, from normal distributions with means 0, 0.5, and 1, each with standard deviation 1.

1. Perform a one-way ANOVA to test whether all three means are equal.
2. Perform three independent two-sample t-tests: samples 1 vs 2, 1 vs 3, and 2 vs 3.
3. Compare the conclusions.

Write a short note on why ANOVA is preferred over running several t-tests.


======


