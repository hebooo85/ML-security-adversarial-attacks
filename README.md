# 🛡️ ML Security — Adversarial Attacks & Defense

> 📚 Machine Learning Security | Fanshawe College

## Overview
Detecting and defending against data poisoning and adversarial 
attacks on CNN classifiers using the MNIST dataset.

## 📊 Results

| Phase | Method | Result |
|-------|--------|--------|
| Baseline CNN | Clean accuracy | 96.65% |
| Data Poisoning | Label-flipping (10%) | 98.47% |
| White-box Attack | PGD L∞ (ε=0.1) | ASR: 7% |
| Black-box Attack | Surrogate PGD | ASR: 3% |
| After Defense | Isolation Forest + Robust CNN | 98.62% |

## 🔬 Attacks Implemented
- **Label-Flipping** — Data poisoning (10% contamination)
- **White-box PGD** — Full gradient access
- **Black-box PGD** — Surrogate model transfer
- **FGM** — Fast Gradient Method

## 🛡️ Defenses
- **Isolation Forest** — Data sanitization
- **Adversarial Training** — PGD-based hardening
- **Randomized Smoothing** — Inference-time defense

## 🛠️ Tech Stack
Python • PyTorch • SecML • Scikit-learn • NumPy • Matplotlib

## 📦 Dataset
MNIST — 70,000 grayscale images (28×28), 10 classes
