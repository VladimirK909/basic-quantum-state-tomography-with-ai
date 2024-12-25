# Basic Quantum State Tomography with AI

This repository contains a basic implementation for **Quantum State Tomography** (QST) for a single, two, and three qubit quantum circuit
using simple **feedforward neural networks** (FNN) and **convolutional neural networks** (CNN).
The training and neural networks is done using **PyTorch** and the quantum circuits are generated and simulated using **Qiskit**.

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
overview

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
├── 3_qubits    		 # Neural network training for a 3 qubit circuit
├── 2_qubit_bell_state   # Neural network training for the 2 qubit Bell state circuit
├── single_qubit.ipynb   # Trivial tomography for one qubit, data generation included
├── circuit_tester.ipynb # Used for visualizing the three quantum circuits
├── requirements.txt     # Python dependencies
└── README.md            # Project documentation
```

## Usage

### The training pipeline
pipeline

### Generating data
data

### Training and evaluation
training and evaluation

## Interesting points
 `interesting points`