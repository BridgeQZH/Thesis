# Thesis

This master thesis is about the application of deep reinforcement learning on Intelligent Transport System(ITS). In detail, I will consider the Traffic Signal Control (TSC) problem.

### Current Situation

The cycle length rarely changes as time goes by.

### Why is it possible now?

We have much richer information that can be collected from various sources.
We have the much stronger computing power.

### Assumptions about the traffic model

### Baselines

Webster, GreenWave, Maxband, Actuated, SOTL, Max-pressure, SCATS

### How to quantify efficiency of the intersection?

- Travel time
- Queue length
- Number of stops
- Throughput


### Why choose deep RL?

RL combined with deep learning, named deep RL, is currently accepted as the state-of-the art learning framework in control systems.

### Challenge

The best approach for optimizing traffic lights is still an open question for researchers, which also proves that the work is meaningful.

### Final product

A system controlling traffic lights with adaptive modules

### Formulation

A single-agent RL problem is modeled as a Markov Decision Process (MDP).

**Environment** is the traffic conditions on the roads.
**Agent** controls the traffic signal.
**Reward** could be defined on the traffic condition of the intersection.

Usually, during the decision process, the policy that the agent takes combines the exploitation of learned policy and exploration of a new policy.




### Implementation problems:

1. When trying to use colab to train the model, I do not know how to edit the ~/.bashrc in order to add the $SUMO_HOME. However, locally some tcpip error about yellowlight happens.

### Why authorities want ITS?

Time saving for drivers, energy saving for environment, and safety for all participants.

### Advanced improvements

Multi-agent RL (MARL)

### Questions(Non-technical):

How to judge the responsibility if accidents happen?
How to prove that autonomous driving will decrease traffic accidents and increase the quality of transportation?

Welcome to discuss in the issues!

### References: (Ranked by importance)

[1] Deep Reinforcement Learning for Intelligent Transportation Systems: A Survey

Part of Abstract: Introduce the latest deep reinforcement learning (RL) based traffic control applications. Specifically, traffic signal control (TSC) applications based on (deep) RL, which have been studied extensively in the literature, are discussed in detail. Different problem formulations, RL parameters, and simulation environments for TSC are discussed comprehensively.   
