# P1 Sandbox

An experimental sandbox for investigating how neural networks can be broken apart and understood, starting with the simplest case: a single-layer network. This is not intended to produce a particular result or solve a defined problem. It is a place to explore an open question: whether neural networks can be sufficiently canonicalized.

The current experiments are deliberately simple and primitive. I am focusing on one-layer networks because, with multiple layers, I found it difficult to isolate the behavior of individual layers from the network's output alone. I plan to expand the experiments as I have more bandwidth.

## Experiments

- **Single-layer tanh network:** Fits a sine function and compares learned parameters and neuron contributions across random seeds.
- **ReLU MLP:** An initial deeper-network experiment using synthetic piecewise functions and visualizations of intermediate layer representations.
- **MARS:** A separate piecewise-linear function-fitting approach for comparison.

## Setup

Requires Python 3, NumPy, Matplotlib, and PyTorch.

```bash
python -m pip install numpy matplotlib torch
```

## Running the experiments

Run scripts from their respective directories:

```bash
cd sine_test
python train_sine.py
```

```bash
cd MLP/ReLu
python neural_network.py
```

```bash
cd MARS/Basic
python basic_mars.py
```
