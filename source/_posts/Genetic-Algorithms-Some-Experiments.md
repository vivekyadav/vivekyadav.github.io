title: 'Genetic Algorithms: Some Experiments'
date: 2015-10-03 19:45:29
tags:
---
These past few months I have been trying out *Genetic Algorithms*.
They are a very interesting, relatively simple but powerful set of algorithms which can be used to find approximate solutions to [NP-hard](https://en.wikipedia.org/wiki/NP-hardness) problems.

Now, a genetic algoeithm can be broken down to these simple steps:
1. Generate a sample population
2. Crossover
3. Mutate

Recursively doing steps 2 & 3 and selecting the healthier candidates at each step, till you don't see improvements across multiple iterations.
The secret is that such algorithms explore a much larger space in a given time period, compared to a deterministic algorithm.
You can find more detailed explainations at other places on the internet so I won't repeat it.
I'll focus a specific aspect, the mutation step.

Just like the crossover part, there are multiple ways to do it. People are experimenting with new ideas.
I got one such idea from a friend of my girlfriend. He called it "Supervised Mutation".
Usually the mutation step is randomized in some way, but he put in a deterministic algorithm. So it is basically combining the powers of randomized and deterministic algorithms.

For some reasons he couldn't take his research to conclusion, but I got interested in it. Hence I have been working on it, along with my girlfriend, during the past few months, although irregularly.

I have the code ready and have been trying to solve some *Travelling Salesman Problem*s, but I need my results to be standardized and comparable to others.
Now how would I do that ? By solving the same problems that others have solved; that way we can compare how efficienct our new algorithm is.
Problem was there are thousands of TSP problems.
Thankfully, I came across something known as [TSPLIB](http://comopt.ifi.uni-heidelberg.de/software/TSPLIB95/). A library of problems including, Symmetric/Asymmetric traveling salesman problem, Hamiltonian cycle problem (HCP), Capacitated vehicle routing problem (CVRP) and some other related category of problems.
Just the thing I was looking for.

So it is still a work in progress and I'll post my findings here, along with code details, later.
But it sure is a refreshing change from what I do at my job at Amazon.