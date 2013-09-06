Financial Analysis in Python
============================

Tutorial at PyData Boston 2013 July 27, 2013 at 4:30 pm.
http://pydata.org/bos2013/schedule/

You can view the video of the talk [here](https://vimeo.com/73875233).

*Thomas Wiecki, Quantopian Inc. and Brown University*

Thomas Wiecki is a Quantitative
Researcher at [Quantopian Inc](https://www.quantopian.com) -- a Boston
based startup providing you with the first browser based algorithmic
trading platform -- and a PhD student at Brown University where he
studies Computational Cognitive Neuroscience. He specializes in
Bayesian Inference, Machine Learning, Scientific Computing in Python,
algorithmic trading and Computational Psychiatry.

Description
-----------

This tutorial will provide hands-on experience of various data
analysis tools relevant for financial analysis in Python. We will
first see how financial data can be imported from various sources such
as Yahoo! finance. Pandas, Matplotlib and statsmodels can be used for
basic and more advanced time-series analysis. While rudimentary
backtesting of investment strategies on historical data can be carried
out using Pandas, a more realistic simulation that considers
transaction costs, slippage and avoids look-ahead bias, introduces
various complexities. We will then see how Zipline, an open-source
streaming-based financial simulator written in Python, can make
realistic backtesting much easier. After going through some simple
example algorithms we will see how statistical Python libraries like
scikits.learn can easily be incorporated with Zipline to build
state-of-the art trading algorithms. Finally, I will briefly show how
the same algorithm code can be run with minimal code changes on
Quantopian -- a free, browser-based platform for developing
algorithmic trading models.

The target audience for the tutorial includes all new Python users,
though we recommend that users also attend the NumPy and IPython
session in the introductory track.

What you will learn
-------------------

* Timeseries analysis using Pandas
* Using Google Trends to predict market movements
* Build your own trading strategies using Zipline
* Common trading strategies:
   * Momentum trading
   * Mean-reversion

Student Instructions
--------------------

For students familiar with Git, you may simply clone this repository
to obtain all the materials (IPython notebooks and data) for the
tutorial. Alternatively, you may [download a zip
file](https://github.com/twiecki/financial-analysis-python-tutorial/archive/master.zip)
containing the materials. A third option is to simply view static
notebooks by clicking on the titles of each section below.

I strongly encourage you to set up the environment on your own
computer so that you can follow along during the tutorial.

After you have the materials, from a command shell cd into the financial-analysis-in-python-tutorial directory and execute:
```
ipython notebook --pylab=inline
```

This should open a new browser window from where you can access the notebooks.

Outline
-------

You can view the video of the talk [here](https://vimeo.com/73875233).

[1. Pandas
basics](http://nbviewer.ipython.org/urls/raw.github.com/twiecki/financial-analysis-python-tutorial/master/1.%2520Pandas%2520Basics.ipynb)
* Creating/Loading time-series data
* Series and DataFrame: First steps
* Data alignment
* Plotting basics
* Common financial analyses (returns, correlations, ...)

[2. Pandas replication of Google Trends
paper](http://nbviewer.ipython.org/urls/raw.github.com/twiecki/financial-analysis-python-tutorial/master/2.%2520Pandas%2520replication%2520of%2520Google%2520Trends%2520paper.ipynb)
* Replication of recent paper: [Quantifying Trading Behavior in Financial Markets Using Google Trends](http://www.nature.com/srep/2013/130425/srep01684/pdf/srep01684.pdf)
* Uses Google search trends to predict market movements

[3. Backtesting using
Zipline](http://nbviewer.ipython.org/urls/raw.github.com/twiecki/financial-analysis-python-tutorial/master/3.%2520Backtesting%2520using%2520Zipline.ipynb)
* What gets modeled? Why?
* Stream-based computing
* My first algorithm
* Example momentum trade algorithm
* Example mean-reversion algorithm

[4. Quantopian: Community, Data, Infrastructure, Live Trading](https://www.quantopian.com)
* Quick intro
* Example algorithm

Required Packages
-----------------

* Python 2.7 (*Python 3 is not supported at this point!*)
* pandas >= 0.11.1
* NumPy >= 1.6.1
* SciPy >= 0.7.0
* Matplotlib >= 1.0.0
* Zipline == 0.5.10

The easiest way to install all the necessary packages (except Zipline) is
to use Continuum Analytics' [Anaconda](http://docs.continuum.io/anaconda/install.html).

Zipline can then be installed via pip:
```
pip install zipline
```
