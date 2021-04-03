# Reinforcement Learning

In this repository we can find some useful reference about reinforcement learning.

"The future is independent of the past given the present"

## Features

* RL problem.

 * observation (Ot) : it is the relevant information of the environment.
 * environment state (St^e) : it is the environment's private representation. It is usually not visible to the agent.
 * agent state (St^a) : it is the agent's internal representation. Any information the agent uses to pick the next action, used by reinforcement learning algorithims.
 * action (At) : task that can be executed by the agent.
 * reward (Rt) : +/- results that receives the agent. For instance, money, positive or negative value.

 * Fully observavibility : Ot = St^e = St^a
 * Partial observability : agent state is different from environment state.


* RL Components.

 * Policy: agent's behavior function. It is a map from state to action.

   * Deterministic policy : a = pi(s)
   * Stochastic policy : pi(a | s) = P[A = a | S = s]. The probability to take the action "a" conditioned by state "s".

 * Value function: how good is each state and/or action. It is a prediction of future reward.

   * State value function (V), and action value funciton (Q)

 * Model: agent's representation of the environment. It predicts what the environment will do next.

   * Transitions (P): predicts the next state (dynamics).  P[S' = s' | S = s, A = a]
   * Rewards (R): predicts the next (immediate) reward. E[R | S = s, A = a]


* Categorizing RL (RL Agent Taxonomy).

   Value example ![Value example](https://github.com/cguz/rl/blob/main/img/value-example.png?raw=true "Value example") 
   
   Policy example ![Policy example](https://github.com/cguz/rl/blob/main/img/policy-example.png?raw=true "Policy example") 
   
   Model example ![Model example](https://github.com/cguz/rl/blob/main/img/model-example.png?raw=true "Model example") 

 * Value Based: Value function and no policy. 

 * Policy Based: No Value function and Policy.

 * Actor Critic: Policy and Value function. 

 * Model Free: Policy and / or Value function. No model.

 * Model Based: Policy and/or Value function. Model.



## Documentation

* [RL Course by David Silver](https://www.youtube.com/watch?v=2pWv7GOvuf0)

* [Reinforcement Learning](http://incompleteideas.net/sutton/book/the-book.html)

* [Algorithms for Reinforcement Learning](https://sites.ualberta.ca/~szepesva/papers/RLAlgsInMDPs.pdf)

## Supervising Master Thesis


