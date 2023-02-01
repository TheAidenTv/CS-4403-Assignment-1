# 1 Pigeon Hole Challenge
## 1.1 Implementation

The way that I decided to implement the pigeon hole challenge, was to
create an empty list that i referred to as domain and then while the domain
list had less than N elements, we generated a random number between 0 and
N-1. If the random number was not in the domain already, we added it to
the domain.

I added a variable, k, to count the number of times a random number
had to be generated before the domain list was full.
Then to repeat this process M times, I put all that code into a for loop
for i in range of M, and added the count value k, to a list called kList for
each iteration.

## 1.2 Run Time
To keep track of the run time I took the system time right before running
the for loop and then again at the end of the for loop then calculated the
difference.

For the original problem of n = 300 and m = 400, the run time was
approximately 2.12 seconds. However, as we increase n and m we can see
that the run time drastically changes and with n = 1500 and m = 1500, it
takes approximately 192 seconds and if we increase the parameters any more
than this the output takes too long for my patience to handle.

## 1.3 Analysis
After repeating the experiment a 1000 times we see that k has a mean
value of 1877.8262, meaning that on average it takes about 1878 random
numbers before we can fill the domain list of size 300. However if the mean
may not be the best estimate of the average; as we see from the graph, there
are a few outliers that sometimes take over 4000 random generations. If
we look at the mode for k its about 1617 random generations which may
be a more accurate way of measuring the most common number of random
numbers it takes to fill the domain.

The highest values I can reasonably reach for n and m before my fans start
spinning and the output takes an unreasonable amount of time, appears to
be whenever n = 1500 and m greater than 1500. This experiment also shows
us that n takes more resources.

Another proof to show that n consumes more resources is in the original
problem, if we make n = 2,000 and keep m = 400, it takes over a minute to
run where as if we switch the values around and do n = 300 and m = 2,000,
it finishes in about 10 seconds.

This also makes sense as n is responsible for the domain size, so as we
increase our domain, it increases the time it takes to fill the domain whereas
increasing m only increases the number of times we repeat the process.

# 2 Birthday Paradox
## 2.1 Implementation
The way that I implemented the second question (Birthday Paradox) was
a similar approach to how he did Lab 1.
