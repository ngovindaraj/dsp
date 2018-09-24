[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

>>
**Code**

t = np.random.random(1000)

pmf = thinkstats2.Pmf(t)

thinkplot.Pmf(pmf, linewidth=0.1)

thinkplot.Config(xlabel='Random variate', ylabel='PMF')

cdf = thinkstats2.Cdf(t)

thinkplot.Cdf(cdf)

thinkplot.Config(xlabel='Random variate', ylabel='CDF')



**Answer**

It seems like the random number generator is close to random as the PMF shows nearly a solid uniform distribution of random values each with probability of 1/1000 or .001 of occurring. Additionally, the CDF shows an almost straight line meaning that the distribution of random numbers appears to almost be uniform.


![Screenshot](4-2a.png)
![Screenshot](4-2b.png)
