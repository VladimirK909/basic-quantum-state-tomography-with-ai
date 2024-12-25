# Basic Quantum State Tomography with AI

This repository contains a basic implementation for **Quantum State Tomography** for a single, two, and three qubit quantum circuit
using simple **feedforward neural networks** and **convolutional neural networks**.
The neural networks and training are done using **PyTorch** and the quantum circuits are generated and simulated using **Qiskit**.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Getting Started](#getting-started)
  - [Installation](#installation)
  - [Repository Structure](#repository-structure)
- [Usage](#usage)
   - [The training pipeline](#the-training-pipeline)
   - [Generating data](#generating-data)
   - [Training and evaluation](#training-and-evaluation)
- [Interesting points](#interesting-points)

## Overview
**Quantum state tomography** (QST) is the process of reconstructing the density matrix of a quantum system (for example, a quantum circuit) using measurement data obtained in different bases. This project shows how QST can be performed using **feedforward neural networks** (FNNs) and **convolutional neural networks** (CNNs).

This repository was created as part of a university course project at the Ss. Cyril and Methodius University in Skopje and provides a simple and intuitive implementation of QST for **1-qubit**, **2-qubit**, and **3-qubit systems**. While most of what is done here is rather trivial in terms of both QST and deep learning, this repository is designed to serve as a well-packaged example for anyone interested in exploring how neural networks can be applied to QST without requiring deep expertise in quantum mechanics, quantum circuits, or artificial intelligence.

The goal is to make QST accessible and comprehensible through **straightforward code and examples**, focusing on delivering the basic idea in a relatively clean and minimalistic manner. Whether you're a beginner curious about QST or an enthusiast looking to experiment with neural networks in quantum computing, this project offers an easy to understand and easily expandable starting point upon which more complex work can be done.

## Features
- Data generation for QST using deep learning
- QST using a FNN for a single qubit (most trivial example)
- QST using a FNN for a two qubit circuit - the Bell state
- QST using a CNN for a two qubit circuit - the Bell state
- QST using a FNN for an arbitrary three qubit circuit
- QST using a CNN for an arbitrary three qubit circuit

## Getting Started
### Installation
1. **Clone the repository**:
   ```bash
   git clone https://github.com/VladimirK909/basic-quantum-state-tomography-with-ai.git
   cd basic-quantum-state-tomography-with-ai
   ```
2. **Install the required dependencies**:
Run the following command:
   ```bash
   pip install -r requirements.txt
   ```
   Alternatively, you can manually install the following packages:
   - **numpy** version 1.26.4
   - **scipy** version 1.13.1
   - **pytorch** version 2.3.1
   - **qiskit** version 0.46.0 
### Repository Structure
```
.
├── data and labels      # .csv files used for the training
├── data generation      # Jupyter notebooks for generating .csv data files
├── 3_qubits             # Neural network training for a 3 qubit circuit
├── 2_qubit_bell_state   # Neural network training for the 2 qubit Bell state circuit
├── single_qubit.ipynb   # Trivial tomography for one qubit, data generation included
├── circuit_tester.ipynb # Used for visualizing the three quantum circuits
├── requirements.txt     # Python dependencies
└── README.md            # Project documentation
```

## Usage

### The training pipeline
```mermaid
flowchart TD;
   A[Start: Measurement Data]-->B;
   B[Data Preprocessing]-->C;
   C[Split Data: Training and Testing Sets]-->D;
   D[Train Neural Networks]-->D1;
   D-->D2;
   D1[Feedforward Neural Network (FNN)]-->E1;
   D2[Convolutional Neural Network (CNN)]-->E2;
   E1[Predict Density Matrix (FNN)]-->F;
   E2[Predict Density Matrix (CNN)]-->F;
   F[Compare with True Density Matrix]-->G;
   G[Calculate Performance Metrics]-->H;
   H[Visualize Results]-->I[End];
```

### Generating data
data

### Training and evaluation
training and evaluation

## Interesting points
 `interesting points`
