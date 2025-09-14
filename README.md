# AI_project_Sharif

AI project phase1 presentation
# Road Segmentation with UNet, Attention UNet, and Residual Attention UNet

This project implements and evaluates three deep learning architectures for road segmentation on the Massachusetts Roads dataset. The models are built from scratch using PyTorch and evaluated using accuracy, IoU score, and Dice score metrics.

## 📋 Project Overview

This repository contains implementations of three semantic segmentation architectures:
1. **UNet** - Baseline encoder-decoder architecture with skip connections
2. **Attention UNet** - UNet variant with attention gates in skip connections
3. **Residual Attention UNet** - Combines residual connections with attention mechanisms

The models are trained and evaluated on the Massachusetts Roads dataset for the task of segmenting roads from aerial imagery.

## 🚀 Features

- **Complete PyTorch implementations** of all three architectures from scratch
- **Robust data pipeline** with proper image-mask pairing and preprocessing
- **Comprehensive evaluation** using multiple metrics (Accuracy, IoU, Dice)
- **Visualization utilities** for comparing predictions against ground truth
- **Self-healing dataset preparation** that handles common data issues

## 📊 Results

| Model | Validation Loss | IoU Score | Dice Score |
|-------|----------------|-----------|------------|
| UNet | 1.0045 | 0.4997 | 0.6632 |
| Attention UNet | 0.99 | 0.50 | 0.66 |
| Residual Attention UNet | 0.89 | 0.58 | 0.72 |

## 🧠 Model Architectures

### UNet
The baseline encoder-decoder architecture with skip connections that preserve spatial information during downsampling and upsampling.

### Attention UNet
Extends UNet with attention gates that help the model focus on relevant regions and suppress irrelevant features in skip connections.

### Residual Attention UNet
Combines residual connections with attention mechanisms to improve gradient flow and feature preservation throughout the network.

## 📈 Performance

All models were trained for 20 epochs with a batch size of 8. The Residual Attention UNet achieved the best performance, demonstrating the value of combining residual connections with attention mechanisms.

## 🎯 Applications

This technology can be applied to:
- Autonomous vehicle navigation systems
- Urban planning and development
- Geographic information systems (GIS)
- Infrastructure monitoring and maintenance
- Emergency response routing

---

# Soft Actor-Critic (SAC) Reinforcement Learning Project

This project implements the Soft Actor-Critic (SAC) algorithm, an off-policy reinforcement learning algorithm that combines maximum entropy reinforcement learning with actor-critic methods. The implementation is tested on the HalfCheetahBulletEnv-v0 environment from PyBullet.

## 📋 Project Overview

This repository contains a complete implementation of the SAC algorithm with:
- **Replay Buffer** for experience replay
- **Actor, Critic, and Value Networks** implemented in PyTorch
- **Training pipeline** with learning curves and model checkpointing
- **Evaluation utilities** for testing trained policies

## 🚀 Features

- **Complete SAC implementation** from scratch using PyTorch
- **Modular neural network architectures** (Actor, Critic, Value networks)
- **Experience replay buffer** for stable off-policy learning
- **Training visualization** with learning curves and score tracking
- **Model checkpointing** for saving and loading trained policies
- **Video recording** capabilities for policy evaluation

## 📊 Results

The SAC implementation successfully learns to control the HalfCheetahBullet environment, achieving scores over 750 after 300 training episodes. The learning curve shows consistent improvement from initial random performance to proficient locomotion.

## 🧠 Algorithm Details

Soft Actor-Critic is an off-policy algorithm that maximizes both expected return and entropy, leading to improved exploration and robustness. Key features include:

- **Maximum entropy framework** that encourages exploration
- **Temperature parameter** that controls the trade-off between exploration and exploitation
- **Two Q-networks** to mitigate overestimation bias
- **Target value network** for stable learning
- **Experience replay** for breaking temporal correlations

## 🎯 Applications

The SAC algorithm can be applied to:
- Continuous control tasks in robotics
- Autonomous vehicle control
- Game AI and character control
- Industrial automation systems
- Physics-based simulation environments

## 📜 Citation

This project was developed by Ali Najar, Mohammad Shafizade, and Armin Khosravi as part of the Artificial Intelligence course in the Computer Engineering Department at Sharif University of Technology, Spring 2025.
