# Optimal Status Update for Caching Enabled IoT Networks: A Dueling Deep R-Network Approach

## Note
File structure: 
1. `AoI_Energy.py` \
   code for environment, which simulates the status update procedure of the concerned IoT network.
2. `dqn.py` \
   code for DQN-based algorithms, i.e., DQ-DSU and DDQ-DSU.
3. `drn.py` \
   code for DRN-based algorithms, i.e., DR-DSU and DDR-DSU.

## Run an experiment
Run **DQ-DSU** in environment with $\gamma=0.95$, $N=24$, $\beta_2=1$ and $P_n=0.6$
``` bash
python dqn.py --Alg dqn --Gamma 0.95 --User 24 --Beta2 1 --Request_P 0.6
```

Run **DDQ-DSU** in environment with $\gamma=0.95$, $N=24$, $\beta_2=1$ and $P_n=0.6$
``` bash
python dqn.py --Alg due --Gamma 0.95 --User 24 --Beta2 1 --Request_P 0.6
```

Run **DR-DSU** in environment with $N=24$, $\beta_2=1$ and $P_n=0.6$
``` bash
python drn.py --Alg dqn --User 24 --Beta2 1 --Request_P 0.6
```

Run **DDR-DSU** in environment with $N=24$, $\beta_2=1$ and $P_n=0.6$
``` bash
python drn.py --Alg due --User 24 --Beta2 1 --Request_P 0.6
```

Evaluation results during training  will be recorded in a tensorboard log file in the current directory.


## Citing 

*C. Xu, Y. Xie, X. Wang, H. H. Yang, D. Niyato, and T. Q. Quek,
“Optimal status update for caching enabled IoT networks: A dueling
deep R-Network approach,” IEEE Trans. Wireless Commun., Jun. 2021,
accepted for publication.*