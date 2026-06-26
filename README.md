<div align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=30&duration=2800&pause=2000&color=F59E0B&center=true&vCenter=true&width=940&lines=Reinforcement+Learning+%F0%9F%A4%96;Multi-Agent+Q-Learning;Teaching+Agents+to+Coordinate" alt="Typing SVG" />
</div>

<div align="center">
  <img src="https://media.giphy.com/media/kH6CqYiquZawmU1HI6/giphy.gif" width="400"/>
</div>

<div align="center">

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![NumPy](https://img.shields.io/badge/NumPy-latest-blue.svg)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)
![Colab](https://img.shields.io/badge/Google-Colab-yellow.svg)

**Teaching multiple agents to coordinate without communication — using only tabular Q-learning**

</div>

---

## 🎮 About This Repository

Reinforcement learning at its core: no neural networks, no function approximation — just a Q-table, a reward signal, and time.

This project explores **multi-agent coordination** in a grid world, where four agents must learn to pick up items and drop them off while avoiding collisions with each other.

```python
environment = {
    "grid_size":    "5 × 5",
    "agents":       4,
    "actions":      ["North", "South", "East", "West"],
    "objective":    "Navigate from pickup A to drop-off B",
    "challenge":    "Avoid collisions with other agents",
    "algorithm":    "Tabular Q-learning (independent learners)",
    "steps":        1_500_000,
}
```

---

## 📂 Project

### 🗺️ Multi-Agent Q-Learning: Grid-World Coordination
`Tabular Q-learning agent.ipynb`

<div align="center">

```
┌─────────────────┐
│  .  .  .  .  .  │
│  .  A  .  .  .  │   A = Pickup point
│  .  .  .  .  .  │   B = Drop-off point
│  .  .  .  B  .  │   ● = Agents
│  .  .  .  .  .  │
└─────────────────┘
  4 agents learn to
  coordinate over
  1.5M environment steps
```

</div>

**What's explored:**
- Independent Q-learners — each agent has its own Q-table
- Collision budget — agents are penalised for occupying the same cell
- Reward shaping — designing rewards that encourage coordination
- Convergence analysis — tracking Q-value updates over training

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aryabhardwaj23/REINFORCEMENT-LEARNING/blob/main/Tabular%20Q-learning%20agent.ipynb)

---

## 📊 Key Concepts Covered

<div align="center">

| Concept | Description |
|---|---|
| **Q-learning** | Off-policy TD control — updating Q(s,a) toward future rewards |
| **ε-greedy exploration** | Balancing exploration vs exploitation over training |
| **Multi-agent setting** | Independent learners in a shared environment |
| **Reward shaping** | Positive reward for successful delivery, penalty for collision |
| **Convergence** | Tracking cumulative reward and collision rate over 1.5M steps |

</div>

---

## 🛠️ Tech Stack

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Google Colab](https://img.shields.io/badge/Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)

</div>

---

## 🚀 Run Locally

```bash
git clone https://github.com/aryabhardwaj23/REINFORCEMENT-LEARNING.git
cd REINFORCEMENT-LEARNING
pip install numpy matplotlib jupyter
jupyter notebook "Tabular Q-learning agent.ipynb"
```

No GPU needed — pure NumPy. Runs in minutes on any machine.

---

## 🔮 What's Next

- Deep Q-Network (DQN) — replacing the Q-table with a neural network
- Policy Gradient methods — REINFORCE and Actor-Critic
- Multi-agent communication — agents that can signal each other

---

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=1,5,10&height=100&section=footer"/>

  **⭐ Star this repo if you enjoyed watching agents learn to cooperate!**

  ![Visitor Count](https://komarev.com/ghpvc/?username=aryabhardwaj23-rl&color=orange&style=for-the-badge&label=VISITORS)
</div>
