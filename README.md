# GridWorld-Q-Learning

## Overview

This project explores reinforcement learning (RL) concepts through a grid-based environment called **GridWorld**. The environment is designed to simulate decision-making scenarios where an agent must navigate from a starting position to a goal while overcoming obstacles, such as walls and doors. The project demonstrates how different RL agents, such as a random agent and a Q-learning agent, interact with the environment and learn optimal strategies.

---

## Objectives

The primary goals of this project are:

1. **Reinforcement Learning Exploration:**
   - Demonstrate how agents learn to navigate an environment using rewards and penalties.
   - Compare the performance of a random agent (no learning) with a Q-learning agent (learning-based).

2. **Dynamic Environment:**
   - Simulate a dynamic environment where obstacles (e.g., doors) can change their state (open/closed) based on probabilities.
   - Highlight how the agent adapts to these changes to find the optimal path.

3. **Pathfinding and Decision-Making:**
   - Show how agents use algorithms like Q-learning to make decisions based on the current state of the environment.
   - Illustrate the trade-off between exploration (trying new paths) and exploitation (choosing the best-known path).

4. **Visualization and Analysis:**
   - Provide visualizations of the agent's behavior and learning process.
   - Analyze metrics such as rewards, steps per episode, and exploration rates to evaluate agent performance.

---

## How It Works

1. **The Environment:**
   - The environment is a 5x5 (10x10) grid where the agent starts at a random position on the bottom row and must reach a goal on the top row.
   - Obstacles include:
     - **Walls:** Fixed barriers that block the agent's movement.
     - **Doors:** Dynamic obstacles that can be open or closed, with probabilities influenced by their position in the shortest path to the goal.

2. **The Agents:**
   - **Random Agent:** Selects actions randomly without learning from the environment.
   - **Q-Learning Agent:** Uses the Q-learning algorithm to learn an optimal policy by balancing exploration and exploitation.

3. **Rewards and Penalties:**
   - The agent receives:
     - **+5** for reaching the goal.
     - **+0.05** for passing through an open door.
     - **-1** for hitting a wall.
     - **-0.1** for normal movement.

4. **Learning Process:**
   - The Q-learning agent updates its knowledge (Q-values) based on the rewards received and the estimated future rewards.
   - Over time, the agent learns to navigate the environment more efficiently, taking fewer steps and achieving higher rewards.

5. **Dynamic Adjustments:**
   - The environment dynamically adjusts door probabilities based on their presence in the shortest path to the goal, encouraging the agent to explore efficient routes.

---

## Key Features

- **Dynamic Obstacles:** Doors that change their state based on probabilities, adding complexity to the environment.
- **Pathfinding:** The agent learns to find the shortest path to the goal while avoiding obstacles.
- **Exploration vs. Exploitation:** The Q-learning agent balances trying new paths with using the best-known paths.
- **Visualization:** Animations and plots to illustrate the agent's learning process and performance.

---

## Getting Started

To run the project, clone the repository and follow the instructions in the provided Jupyter Notebook or Python scripts. The project includes visualizations and metrics to help you analyze the agent's behavior and learning process.

---

## Future Work

Potential extensions of this project include:

- Adding more complex obstacles or dynamic elements to the environment.
- Implementing additional RL algorithms, such as SARSA or Deep Q-Learning.
- Scaling the environment to larger grids or continuous spaces.
- Introducing multi-agent scenarios for collaborative or competitive tasks.

---

## Acknowledgments

This project is inspired by reinforcement learning concepts and aims to provide an interactive and visual way to understand how agents learn to make decisions in dynamic environments.
