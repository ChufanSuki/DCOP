## The Distributed Stochastic Algorithm
- synchronous execution model
- stochastic decision on whether agents should actually perform a move when they see the opportunity to optimize the gain

Pseudocode:
1. Initialization phase(choose random values)
2. Loop
    1. At each execution step, each agent $$A_i$$ executes the following operations
        - Choose an activation probability $$p_i \in [0,1]$$
        - Generate a random number $$r_i \in [0,1)$$
        - If $$r_i < p_i$$ choose a value ai such that the local gain is maximized
        - If $$r_i \geq p_i_$$ do not change its value
        - If the variable value changed, send information to all neighbors notifying them of the change
        - Receive messages from neighbors and update information accordingly