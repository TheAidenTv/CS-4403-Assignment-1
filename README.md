# Assignment 1

## The Pigeon Hole Challenge

Consider a domain of size n = 300. 

Generate random numbers in the domain [n] until every value i ∈ [n] has had one random number equal to i. 

How many random trials did this take? 

We will use k to represent this value. 

Repeat 400 times (let's call this counter m), and for each repetition record k. 

Make a density plot.

What can you say about k? 

Describe how you implemented this experiment and how long it took for n = 300 and m = 400 trials. 

Show a plot of the run time as you gradually increase the parameters n and m.   Go to https://matplotlib.org/ to learn how to create visualizations in Python. 

Now have some fun and try some different values for n and m. 

What are the highest values for n and m that you can reasonably reach?  Which one claims the most resources? Why?

## The Birthday Paradox

Consider a domain of size n = 5000. 

Generate random numbers in the domain [n] until two have the same value. 

How many random trials did this take? 

We will again use k to represent this value. 

Repeat the experiment m = 300 times, and record k each time. 

Make  a density plot. The plot should show a curve that starts at a y value of 0, and increases as k increases, and eventually reaches a y value of 1. 

What can you say about k?

Describe how you implemented this experiment and how long it took for m = 300 trials. Show a plot of the run time as you gradually increase the parameters n and m. 

What are the highest  values for n and m that you can reasonably reach?

## Finding Similar Sentences

I used GPT-3 to generate a bunch of sentences of various lengths. You can find the results in the following files:
- [100 very short sentences](https://github.com/TheAidenTv/CS-4403-Assignment-1/blob/main/Random%20very%20short%20sentences.txt)
- [100 short sentences](https://github.com/TheAidenTv/CS-4403-Assignment-1/blob/main/Random%20short%20sentences.txt)
- [100 long sentences](https://github.com/TheAidenTv/CS-4403-Assignment-1/blob/main/Random%20long%20sentences.txt) 
- [100 Spanish sentences](https://github.com/TheAidenTv/CS-4403-Assignment-1/blob/main/Random%20spanish%20sentences.txt)

Within each document, construct k-grams for all sentences (you will want to convert upper case to lower case), as follows:
- character based 2-grams
- character based 3-grams 
- word based 2-grams 

You should only store each k-gram once, duplicates are ignored. 

How many distinct k-grams are there for each document with each type of k-gram? 

Compute the Jaccard similarity between all pairs of sentences for each type of k-gram within each document.  

Report for each document the 5 pairs of sentences which are the most similar.

What can you state about the computational cost for this experiment?
