[RL Code](https://colab.research.google.com/drive/1ZNv9QmQQaPfvOjZLgmbE_hAcp7ZQhRJY?usp=sharing)

Explanation :-
    Reinforncement Learning: The model learns the optimal behavioral pattern to a solution through reacting to the environment , updating result (reward if positive or punishment if negative) and repeating this process over and over again and finds out actions with the largest long-term reward and follows those actions.

Some Terms :- 
  1) Agent :- The learner which takes actions
  2) Environment :- The world the agent interacts with
  3) State :- A description of the environment at a given moment of time
  4) Action:- A choice the agent makes
  5) Reward :-A positive feedback signal recieved after a correct action
  6) Policy :- A strategy that matches states and actions
  7) Exploration vs Exploitation :- Balancing trying new actions to learn and using known actions

Q-Learning:- Its a model-free reinforcement learning algorihm that enables an agent to learn the best policy for an environment that relies on the Bellman equation that updates values for actions taken.
    Equation:-
                Q(s,a)←Q(s,a)+α[r+γ*maxQ(s′,a′)−Q(s,a)]
    Q(s,a) = Current estimate of value in state s by taking action a
    α = Learning Rate -> Determines how much new information updates the old info
    r = Reward recieved after performing action
    γ = Discount Factor --> Weighs importance of future rewards relative to immediate ones
    max() = Best estimated future reward obtainable from state s'
    s' = Next state reeached by taking action a

Hyperparametre:-
1) Learning Rate (α) = Controls how fast Q-Values are updated. A high rate means rapid learning but more instability.
2) Discount Factor (γ) = Higher factor makes agent long-sighted
3) Exploration Rate (ε) = Controls Exploration vs Exploitation. Decays over time
4) Episodes:- Number of iterations for training
5) Reward Function:- Defines feedback signal shaping behaviour
    
