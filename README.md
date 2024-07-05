# DQN-AC-LunarLander
In this project the goal is to solve the lunar lander game, which means the lander needs to land safely with two of the spaceship's legs on the ground, between the two flags.
For full documentation of the game and more games you are invited to visit gymnasium website: https://gymnasium.farama.org/environments/box2d/lunar_lander/
(Animation of the DQN model solving the game is added at the end).

We will see the difference between the Reinforcement Learning methods of DQN (Deep Q Network) and AC (Actor Critic).

The DQN model is a value based method being updated trought a "Q step" that updating Q (the state-action reward function).
Q step:

![image](https://github.com/RanMatalon/DQN-AC-LunarLander/assets/138029692/edec9165-d27c-45b9-8d15-c535420f6eab)

The DQN optimizer:

![image](https://github.com/RanMatalon/DQN-AC-LunarLander/assets/138029692/7c3e3141-c8c4-48f8-ad93-375c5d1ceb2d)


Thats while the AC is a policy gradient method that is seperated to the Actor who is responsible for updating the Likelihood ratios accordingly to the actor loss.
Policy gradient:

![image](https://github.com/RanMatalon/DQN-AC-LunarLander/assets/138029692/e209ae0f-4185-44e6-9e07-40de206ed548)

Another optimizing component is the critic loss that critisizes every action we do and makes sure it yields a positive reward (advantage).

The AC model:

![image](https://github.com/RanMatalon/DQN-AC-LunarLander/assets/138029692/a5db2035-f040-4340-8ae3-695807543446)

By the results that both methods yield it can be seen that DQN yields better reward but with higher variance, in contrast to AC that yields lower rewards but lower variance.

Animation of the DQN model:

https://github.com/RanMatalon/DQN-AC-LunarLander/assets/138029692/00424ab8-9cc5-49c1-94c9-cee2c810b5e3


