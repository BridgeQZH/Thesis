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

- The best approach for optimizing traffic lights is still an open question for researchers, which also proves that the work is meaningful.
- Optimizing the travel time of all vehicles in the network becomes especially harder when the destination of a vehicle in unknown to the traffic signal controller in advance.
- Design of RL formulation; The weight on each term is tricky to set.
- Learning efficiency.
- Credit assignment. In order to maximise the reward in the long run, the agent needs to determine which actions will lead to such outcome, which is essentially the temporal CAP.
- Safety issue

### Final product

A system controlling traffic lights with adaptive modules

### Formulation

A single-agent RL problem is modeled as a Markov Decision Process (MDP).

**Environment** is the traffic conditions on the roads.
**Agent** controls the traffic signal.
**State** include components such as queue length, number of cars, waiting time, and current traffic signal phase; images of vehicles’ positions on the roads;  Volume; Delay; Speed; Phase duration.

- Queue length

of a lane is the total number of waiting vehicles on the lane

- Waiting time

of a vehicle is defined as the time period a vehicle has been in the “waiting” state

- Volume

of a lane is defined as the number of vehicles on the lane, which equals to the sum of queuing vehicles and moving vehicles on the lane.

- etc

**Reward** could be defined on the traffic condition of the intersection. A typical reward definition is a weighted linear combination of several components such as queue length, waiting time and delay. **Travel time** is hard to serve as an effective reward in RL for several reasons.

- Queue length
- Waiting time
- 

### Multi-Agent Difference

The reward could be defined on the level of individual intersections or a group of intersections within the environment.
Coordination strategy



### Implementation problems:

1. When trying to use colab to train the model, I do not know how to edit the ~/.bashrc in order to add the $SUMO_HOME. However, locally some tcpip error about yellowlight happens.

### Why authorities want ITS?

Time saving for drivers, energy saving for environment, and safety for all participants.

### Simulation environment

Simulation of Urban MObility (SUMO): an open-source program for traffic simulation; API called TraCI; can be accelerated by allowing a version without a graphical interface;  supports other upper-level computational frameworks for deep RL and control experiments for traffic microsimulation.

### Advanced improvements

Multi-agent RL (MARL)

### Questions(Non-technical):

How to judge the responsibility if accidents happen?
How to prove that autonomous driving will decrease traffic accidents and increase the quality of transportation?

Welcome to discuss in the issues!

### References: (Ranked by importance)

[1] Deep Reinforcement Learning for Intelligent Transportation Systems: A Survey

Part of Abstract: Introduce the latest deep reinforcement learning (RL) based traffic control applications. Specifically, traffic signal control (TSC) applications based on (deep) RL, which have been studied extensively in the literature, are discussed in detail. Different problem formulations, RL parameters, and simulation environments for TSC are discussed comprehensively.   
