Reinforcement Learning Basics
==============

This is for basic reinforcement learning: algorithms and main equations for dynamic programming (DP), monte carlo method (MC), temporal difference (TD) and deep reinforcement learning (DRL). The task of the robot is to collect data of all sensors in the shortest possible time while it avoids any collisions to the obstacles.

Details
-----

### 0. Grid Environments

* 5x5 grid env. (grid_env_55.ipynb)   
    * Fast convergence, **recommended!!!**
* 10X10 grid env. (grid_env.ipynb)   
    * Slow convergence   


### 1. Dynamic Programming (DP)

* There are two versions of DP: state value based and action value based
* Policy evaluation, policy improvent
* Policy iteration
* Value iteration

### 2. Monte Carlo Method (MC)

* On-policy first visit MC
* Off-policy first visit MC

### 3. Temporal Difference (TD)

* SARSA, Q-learning, Expected SARSA, Double Q-learning


### 4. Deep Reinforcement Learning (DRL)
We have a robot that aims to collect data of several low-powered IoT sensors. As the sensors are low-powered, they cannot communcate over long ranges. Hence, the robot must approach each sensor to collect their data. The robot starts its mission from the start terminal. There is a charging station in the environment so that the robot can recharge its battery if it is running out of energy. Also, there are several obstacles in the environment. 



A sample result:

-----

### Value Functions (State value $V(s)$, Action value $Q(s,a)$ )
<p align="left">
    <img src="./results/state_value.png" width="300" height="300">
    <img src="./results/action_value.png" width="300" height="300">
</p>

### 10x10 Grid Environment
<img src="./results/env.png" width="200" height="200">


In the following image, we have depicted the environment:

<img width="296" alt="Env" src="https://user-images.githubusercontent.com/37718565/167018071-d82d1445-17e9-4b01-9604-d7c2339bbd8e.png">

red square: starting position

green square: charging station

Black circles: IoT sensors

Blue blocks: obstacles


In this project, we define the state as a four channel image, shown below

<img width="865" alt="img" src="https://user-images.githubusercontent.com/37718565/167021810-200d8550-21e6-4540-ab24-c8fac41e23ef.png">

Based on this definition, we can use CNNs to solve the MDP. 



<img width="296" alt="res" src="https://user-images.githubusercontent.com/37718565/167018611-38facc53-ab32-42f8-99b9-014151581baa.png">
