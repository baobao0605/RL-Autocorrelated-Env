# RL for Memory Strategies in Autocorrelated Environments

## 项目简介 (Project Overview)
本项目旨在通过强化学习（Reinforcement Learning）算法，训练智能体在具有**自相关性（Autocorrelation）**的环境中，学会选择最优的记忆策略——即何时进行**编码（ENCODE）**，何时进行**提取（RETRIEVE）**。

环境构建的核心思路参考了 Qihong Lu (吕其鸿) 教授的研究，在此基础上，本项目设计并实现了多个不同层级的强化学习算法，以观察智能体策略的演化过程和性能差异。

## 目录结构 (Repository Structure)
所有的核心代码与实验结果均保存在 `experiments/` 目录下，采用 Jupyter Notebook 格式，便于展示交互式的训练过程和图表。

```text
├── experiments/
│   ├── 01_REINFORCE/                # 基础策略梯度算法
│   ├── 02_Actor_Critic_NonNeuro/    # 无神经网络的 Actor-Critic (Tabular/Linear)
│   ├── 03_Actor_Critic_HiddenLayer/ # 带单隐藏层的 Actor-Critic
│   ├── 04_Signal_Specific_Strategy/ # 基于不同信号分离策略的针对性训练
│   └── 05_GAE_Actor_Critic/         # 结合广义优势估计 (GAE) 的 Actor-Critic
├── README.md
