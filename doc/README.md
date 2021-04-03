# Features Learned

Here I add some notes about the course that I have read. 

# Table of Content

* [RL Course by David Silver](#RL_DAVID_SILVER)


## RL Course by David Silver <a name="RL_DAVID_SILVER"></a>    

The link of the course (:movie_camera:) can be found in [RL Course by David Silver](https://www.youtube.com/watch?v=2pWv7GOvuf0)

All the slides are in the (:file_folder:) 'David-silver'. 

### RL problem.

 * observation (Ot): it is the relevant information of the environment.
 * environment state (St^e): it is the environment's private representation. It is usually not visible to the agent.
 * agent state (St^a): it is the agent's internal representation. Any information the agent uses to pick the next action, used by reinforcement learning algorithms.
 * action (At): a task that can be executed by the agent.
 * reward (Rt): +/- results that receive the agent. For instance, money, positive or negative value.

 * Fully observavibility : Ot = St^e = St^a
 * Partial observability : agent state is different from environment state.
 

### RL Components.

 * Policy: agent's behavior function. It is a map from state to action.

   * Deterministic policy : a = pi(s)
   * Stochastic policy : pi(a | s) = P[A = a | S = s]. The probability to take the action "a" conditioned by state "s".

 * Value function: how good are each state and/or action. It is a prediction of future rewards.

   * State value function (V), and action-value function (Q)

 * Model: agent's representation of the environment. It predicts what the environment will do next.

   * Transitions (P): predicts the next state (dynamics).  P[S' = s' | S = s, A = a]
   * Rewards (R): predicts the next (immediate) reward. E[R | S = s, A = a]


### Categorizing RL (RL Agent Taxonomy).

First of all, let us see one example of Value, Policy, and Model. 

   Value example:
   
   ![Value example](https://github.com/cguz/rl/blob/main/img/value-example.png?raw=true "Value example") 
   
   Policy example:
   
   ![Policy example](https://github.com/cguz/rl/blob/main/img/policy-example.png?raw=true "Policy example") 
   
   Model example:
   
   ![Model example](https://github.com/cguz/rl/blob/main/img/model-example.png?raw=true "Model example") 

With this in mind, we can categorize an RL Agent as:

 * Value-Based: Value function and no policy. 

 * Policy Based: No Value function and Policy.

 * Actor-Critic: Policy and Value function. 

 * Model Free: Policy and/or Value function. No model.

 * Model-Based: Policy and/or Value function. Model.

