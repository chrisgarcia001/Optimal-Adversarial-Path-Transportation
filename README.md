Optimal Transportation of Critical Items Over Hostile Paths
===============
### Optimal multiunit transfer over adversarial paths with increasing intercept probabilities
This repo contains the code and experimental results used in the research paper 
[*Optimal multiunit transfer over adversarial paths with increasing intercept probabilities*] (https://www.tandfonline.com/doi/abs/10.1080/24725854.2018.1488306) by C. Garcia.
This research addresses the problem of optimally transporting a set of items over a set of hostile paths where an adversary seeks to intercept them. 
Each item leaves a certain footprint on a path as it crosses, and the probability of an item being intercepted on a given path increases as the 
cumulative footprint on that path increases (i.e. the more items that have already crossed, the more likely an item is to be intercepted when crossing).
Specifically, each path has a monotonically decreasing intercept probability function that specifies the probability of an item being intercepted
with respect to cumulative footprint. The objective is to both allocate a set of items to each path and sequence them to maximize the probability that
all items successfully reach their destination. 

#### Solution Approach
In the paper this problem was proven to be strongly NP-hard. Accordingly, exact approaches may be employed only for small problem instances. Accordingly, four 
optimization algorithms were developed: 

1. An exact enumerative algorithm
2. A greedy heuristic
3. A greedy heuristic combined with local search
4. A genetic algorithm

The greedy heuristic with local search proved to be the most robust, achieving the best solutions on larger problems while having shorter run times than the GA

#### Code Organization and How to Run



#### Paper and Citation
The full paper can be found [here.](https://www.tandfonline.com/doi/abs/10.1080/24725854.2018.1488306)
If you wish to cite this work, please use the following reference:
Christopher Garcia, "Optimal multiunit transfer over adversarial paths with increasing intercept probabilities", IISE Transactions, Vol. 50 Iss: 11, pp.989-996.

