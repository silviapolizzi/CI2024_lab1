# Lab 1 Computational Intelligence
## Set Cover Problem description
The **Set Cover Problem** involves a universe of elements and a collection of sets, each containing some of these elements. The goal is to select the fewest sets (or minimize the total cost of selected sets) such that every element in the universe is covered by at least one selected set. This problem is NP-hard, meaning it's computationally difficult to find an optimal solution for large instances.

---
## Algorithms implemented
I tried three different algorithms to solve the Set Cover problem:
1. **Hill Climbing** with multiple mutations: in this version of hill climbing, multiple mutation are applied to the current solution during each iteration, and the strength of these mutations (the number of mutations) is decreased as iterations progress.
2. **Simulated Annealing**: this algorithm  allowing the algorithm to escape local optima by accepting worse solutions with a probability that decreases as the algorithm progresses.
3. **Tabu Search**: this approach avoid revisiting recently explored solutions, which helps to escape local optima.

The algorithms were tested on a set of 6 instances of the Set Cover problem, with the following characteristics:
### Instances
|# INSTANCE| Universe size| Number of sets | Density|
|----------|----------|----------|----------|
| 1 | 100 | 10 | 0.2|
| 2 | 1_000 | 100 | 0.2|
| 3 | 10_000 | 1_000 | 0.2|
| 4 | 100_000 | 10_000 | 0.1|
| 5 | 100_000 | 10_000 | 0.2|
| 6 | 100_000 | 10_000 | 0.3|

## Discussion
After testing these algorithms, **Hill Climbing** was selected as the best trade-off in terms of solution cost, runtime performance, and the number of function calls.  

## Results


| # INSTANCE | Best fitness | # OF CALLS |
|----------|----------|----------|
| 1 | -292.92 | 0 |
| 2 | -7689.43 | 19   |
| 3 | -741479.28| 292  |
| 4 | -112751635.59 |  435 |
| 5 |  -238795309.18 |  489 |
| 6 | -370743077.11 | 474  |

