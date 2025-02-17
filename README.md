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

## 🖥 How to Run
### 1️⃣ Install Required Libraries
```bash
pip install numpy matplotlib
