# Adaptive Reinforcement Learning Defense Framework Against Cryptographic Cross-Model Adversarial Prompt Injection

This project introduces an **Adaptive RL-based Defense Framework** to combat **Cryptographic Cross-Model Adversarial Attacks** in Large Language Models (LLMs). The framework operates in a dynamic game-theoretic setting where:

- **Adversaries** use cryptographic ciphers to generate adversarial prompts that exploit vulnerabilities across multiple LLMs.
- **Defenders** deploy reinforcement learning (RL)-based strategies to adaptively decode ciphers, mitigate adversarial effects, and maintain robust LLM performance.

The project aims to create a resilient framework capable of adapting to varying attack patterns and ensuring LLM robustness while preserving model accuracy and response quality.

---

## Key Features

1. **Cryptographic Adversarial Prompts:**
   - Dynamically generated cipher-encoded adversarial prompts.
   - Cross-model transferability analysis of adversarial attacks.

2. **Reinforcement Learning Defense Mechanism:**
   - Adaptive RL agent learns to decode and neutralize cipher-based adversarial prompts.
   - Holistic agent setup includes an external defender modules in the form of an independent LLM that learns to decode the ciphered prompts and expose the adversary.

3. **Dynamic Adversarial-Defense Framework:**
   - Attackers dynamically change ciphering strategies, challenging the defense agent.
   - Defender iteratively improves the decoding through an adaptive learning mechanism that uses other external LLMs as judges to rate (reward) the decoded prompt.

4. **Evaluation Metrics:**
   - Attack Success Rate (ASR)
   - Benign Success Rate (BSR)

---

## Installation

### Prerequisites
- Python 3.9+
- GPU (recommended for RL model training)

### Steps
1. Clone the repository:
   ```shell
   git clone https://github.com/latentghost/rl-defense-against-cryptographic-adversarial-attack.git
   cd rl-defense-against-cryptographic-adversarial-attack
   ```
2. Install dependencies:
   ```shell
   pip install -r requirements.txt
   ```
3. 