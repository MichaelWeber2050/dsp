[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

>>random_nums = np.random.random(1000)
pmf = thinkstats2.Pmf(random_nums)
thinkplot.Pmf(pmf, linewidth=.1)
thinkplot.Config(xlabel='Random num', ylabel='PMF')

yields a nearly fully filled graph.

Probability mass function (PMF): a representation of a distribution as
a function that maps from values to probabilities.
# answer
Every number has an equal probability to be selected thus each number has the same correlation 
from values to probabilities

cdf = thinkstats2.Cdf(pmf, label='random nums')
thinkplot.Cdf(cdf)
thinkplot.Show(xlabel='random nums', ylabel='CDF')

Yes it is nearly a straight line so the distribution is uniform 
