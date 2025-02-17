# Q-Learning GridWorld 🚀

This project implements **Q-Learning** to train an agent in a GridWorld environment with obstacles.  
The agent learns to navigate from the **start state** to the **goal state** while avoiding obstacles.

## 📌 Project Overview
- **Algorithm**: Q-Learning (Off-policy Temporal Difference Control)
- **Environment**: 4x7 GridWorld with obstacles
- **Objective**: Learn an optimal policy for the agent to reach the goal
- **Rewards**:
  - Normal movement: `-1`
  - Hitting an obstacle: `-100`
  - Reaching the goal: `+100`
  - Going out of bounds: `-10`

## 🔍 Key Features
- 📌 Environment Setup
  - grid_size: 4x7 grid
  - obstacles: Predefined obstacle locations
  - start_state: (0,0)
  - goal_state: (3,6)
- 📌 Q-Learning Algorithm
  - Exploration vs Exploitation (ε-greedy)
  - Q-table Update:
    - $𝑄(𝑠,𝑎)=𝑄(𝑠,𝑎)+𝛼[𝑅+𝛾max𝑄(𝑠′,𝑎′)−𝑄(𝑠,𝑎)]Q(s,a)=Q(s,a)+α[R+γmaxQ(s′,a′)−Q(s,a)]$
    - Epsilon Decay: ε = max(ε_min, ε * decay)
- 📌 Visualization
  - Uses matplotlib to display the optimal policy as a grid
  - Marks:
  - Start (S)
  - Goal (G)
  - Obstacles (X)
  - Optimal actions (↑, ↓, ←, →)
### 1️⃣ Install Required Libraries
```bash
pip install numpy matplotlib
