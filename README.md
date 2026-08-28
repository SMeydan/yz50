# YZ50 — From Neural Networks to GPT

My implementations, experiments, and technical notes from **YZ50**, a 12-week AI research program focused on building neural networks and language models from scratch.

The program follows Andrej Karpathy's *Zero to Hero* approach: instead of treating deep learning frameworks as black boxes, I am rebuilding the underlying concepts step by step — from a single neuron and gradient descent to autograd, language models, backpropagation, and eventually a small GPT system.

> **Goal:** Understand how neural networks and language models work by implementing them from the ground up.

🔗 **Program:** [yz50.ai](https://yz50.ai/)

---

## Progress

| Week      | Topic                                 | Status         |
| --------- | ------------------------------------- | -------------- |
| **01**    | Neural Networks & Gradient Descent    | ✅ Completed    |
| **02**    | micrograd & Automatic Differentiation | 🔄 In progress |
| **03**    | PyTorch Fundamentals                  | ⬜ Upcoming     |
| **04**    | makemore & Language Modeling          | ⬜ Upcoming     |
| **05**    | Embeddings & MLP Language Models      | ⬜ Upcoming     |
| **06**    | Training Mechanics & Debugging        | ⬜ Upcoming     |
| **07**    | Backprop Ninja                        | ⬜ Upcoming     |
| **08**    | WaveNet & Deep Architectures          | ⬜ Upcoming     |
| **09–12** | Transformers, GPT & Capstone          | ⬜ Upcoming     |

---

## Week 01 — Neural Networks

The first week focused on understanding the basic mechanics behind a neural network before relying on frameworks such as PyTorch.

### Implemented

* Single neuron forward pass
* Parameters, weights, and bias
* Activation functions
* Loss calculation
* Manual parameter updates
* Gradient descent intuition
* Basic experiments around how parameter changes affect loss

### Notes

I also wrote a short technical note explaining how a model learns through the interaction between:

```text
Input
  ↓
Neuron
  ↓
Activation
  ↓
Prediction
  ↓
Loss
  ↓
Gradient
  ↓
Parameter update
  ↺
```

The goal was not to build a useful model yet, but to understand the mechanics that later become automated by autograd frameworks.

---

## Week 02 — micrograd & Automatic Differentiation

**Currently working on this week.**

The focus is moving from manually reasoning about individual derivatives to building a small scalar automatic differentiation engine.

### Concepts

* Computational graphs
* Derivatives
* Chain rule
* Backpropagation
* Scalar autograd
* Topological sorting
* Gradient accumulation

### Implementation goals

* [ ] Implement a `Value` object
* [ ] Track computational graph dependencies
* [ ] Implement addition
* [ ] Implement multiplication
* [ ] Implement power
* [ ] Implement `tanh`
* [ ] Implement backward propagation
* [ ] Build topological ordering
* [ ] Train a small MLP
* [ ] Compare gradients against numerical derivatives

---

## Why I'm Doing This

Modern deep learning frameworks make training neural networks accessible, but abstraction can also hide the mechanics underneath.

This repository is my attempt to work in the opposite direction:

**start with the fundamentals → implement the machinery → understand the abstraction.**

By the end of the program, the goal is to have implemented the major building blocks behind a small language model and understand what happens beneath high-level APIs.

---

## Repository Structure

```text
yz50/
├── week1.py        # Week 1 neural network experiments
├── notes.html      # Interactive learning notes
├── style.css       # Styling for the notes
├── week2.py        # Week 2 autograd implementation
└── README.md
```

The structure will evolve as the program progresses.

---

## Learning Log

This repository is intentionally kept as a **work in progress**.

I will document:

* What I implemented
* What I learned
* Experiments and observations
* Bugs and debugging decisions
* Training results
* Technical notes
* Weekly checkpoints

The goal is to preserve the process, not just the final code.

---

## References

* [YZ50 — Türkiye'nin Yapay Zeka Araştırmacıları](https://yz50.ai/)
* [Andrej Karpathy — Zero to Hero](https://karpathy.ai/zero-to-hero.html)
* [micrograd](https://github.com/karpathy/micrograd)

---

<div align="center">

**Learning by building from first principles.**

</div>
