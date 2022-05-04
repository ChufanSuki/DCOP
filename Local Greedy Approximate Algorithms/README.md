## Local Greedy Approximate Algorithms
- Start with a randomn assignment for all the variables
- Local moves
    - change the value of a small set of variables
    - difference on objective after change called gain
- Stop when no positive gain

Advantages:
- little memory and computation

Problem:
- local optimal

Heuristic solution:
- Stochastic Local Search(random restart)
- walkSAT and Simulated Annealing(stochastic steps in the search process)

Incoherence problem when applied to DCOP. If all agents are allowed to execute in parallel, each agent has out-of-date knowledge about the choices of other agents.