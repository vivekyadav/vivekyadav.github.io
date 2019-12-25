title: Stuck at the locality
date: 2016-01-13 19:45:29
tags:
---


In [my previous post](http://www.vivek.nl/2015/10/03/Genetic-Algorithms-Some-Experiments/), I mentioned about working on a new type of genetic algorithm.
I went ahead and completed the program and tested it against data sets taken from [TSPLIB](http://comopt.ifi.uni-heidelberg.de/software/TSPLIB95/).

At first the results were promising, especially on the ATT48 dataset, but on trying out other data sets, I realized my algorithm was getting stuck at local minima. I tried increasing the population size and various combination of parameters but it would still end up in a minimum.

I left it at that point for some time. Recently, I have started work on it again.
There is something known as Niching in Genetic Algorithms. I plan to use it in my algorithm and see if there is any improvement (I hope there is).

By the way, coming to the programming language for this, it’s all in C++; had to be, if it’s CPU intensive then there is only 1 language for me, C++. The standard library has been good enough for me, except for logging. For that purpose, I have used [spdlog](https://github.com/gabime/spdlog).

