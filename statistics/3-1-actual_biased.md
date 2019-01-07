[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

>> This problem presents a robust example of actual vs biased data. As a data scientist, it will be important to examine not only the data that is available, but also the data that may be missing but highly relevant. You will see how the absence of this relevant data will bias a dataset, its distribution, and ultimately, its statistical interpretation.

resp = nsfg.ReadFemResp()

actual = resp.numkdhh
pmf = thinkstats2.Pmf(actual, label='actual')
print('mean', pmf.Mean())

def BiasPmf(pmf, label):
    new_pmf = pmf.Copy(label=label)
    for x, p in pmf.Items():
        new_pmf.Mult(x, x)
thinkplot.Show(xlabel='Number of kids', ylabel='PMF')

thinkplot.PrePlot(2)
thinkplot.Pmfs1.024205

diff = biased_pmf.Mean() - pmf.Mean()
print('difference in actual vs biased =', diff)
print('or ', diff/pmf.Mean()*100, '%')

difference in actual vs biased = 1.3794739456204508
or  134.68726834922208 %
