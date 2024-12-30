---
marp: true
theme: default
header: Brain Sciences and Brain Disorders 2024 Fall
footer: Group 10：刘思昀、虞果、唐林峥
paginate: true
math: katex
---

# Intelligent Brain Organoid

Developing Functional Neural Networks in Brain Organoids with FEP

---

# Catalog

1. ### Introduction
1. ### Background
1. ### Proposed Methodology

---

# Introduction

## Understanding Brain Organoids

An **artificially grown**, **in vitro**, tissue resembling parts of the human brain.

![bg right:40% fit](image/slides/brain-organoids-flow.png)

---

# Introduction

## Understanding Brain Organoids

The purpose: *to study related diseases in a more defined setting*.

![bg right:40% fit](image/slides/brain-organoids-flow.png)

---

# Introduction

## What's the Barriers?

- Physically hard to construct.

- Functionally hard to develop.

![bg right:40% ](image/slides/barin-complexity.png)


---

# Introduction

## Possible Solution

- Physically: Focusing on reconstructing a **specific brain region**.

![bg right fit](image/slides/barin-anatomy.png)

---

# Introduction

## Possible Solution

- Functionally: **Actively "train"** the organoid besides natural development.

![bg right:60% fit 95%](image/slides/demo-dishbarin.png)

---

# Background
## Reconstruct Specific Region

Lot's of previous work could be referred directly.

![bg right:50% fit 97%](image/slides/brain-organoids-regisons.png)

---

# Background
## Free Energy Principle

- Author: Karl Friston (2010)
- A normative theory on **living organism's** intelligence
- Derived from a specific form of **variational bayesian inference**.

![bg right:40%](image/slides/karl-friston.webp)


---

<div style="margin-top: 100px"></div>

# Background
## Free Energy Principle
  - Bayesian Brain Hypothesis.
  - Self-Organized System **minimize** it's **free energy (surprise)**.

<style>
  .scaled-down-math {
    transform: scale(0.85);
    transform-origin: top left;
    margin-left: 10%;
  }
</style>

<div class="scaled-down-math">

$$
\begin{align*}
\underbrace{F(\mu, a; s)}_{\text{free-energy}} &= \underbrace{\mathbb{E}_{q(\psi)} \left[ -\log p(\psi, s, a, \mu \mid \psi) \right]}_{\text{expected energy}} - \underbrace{\mathcal{H}[q(\psi \mid s, a, \mu, \psi)]}_{\text{entropy}} \\
&= \underbrace{-\log p(s)}_{\text{surprise}} + \underbrace{\text{KL}[q(\psi \mid s, a, \mu, \psi) \parallel p_{\text{Bayes}}(\psi \mid s, a, \mu, \psi)]}_{\text{divergence}} \\
&\geq \underbrace{-\log p(s)}_{\text{surprise}}
\end{align*}
$$

</div>

---

# Background
## Free Energy Principle

- Internal and external state are separated by **markov blanket**.

- Brain makes **variational bayesian inference**. 

- Brain fitting the world **as precise as possible**.

![bg right:45% 95%](image/slides/fep-demo.jpg)

---

# Background
## Dish Brain

Training a BNN playing video game **based on FEP theory**.

![bg right:55% ](image/slides/absract-dishbrain.jpg)

---


# Proposed Methodology

- Reconstruct organoid of a specific brain region in **marco** morphology with emergence of the markers.

- Using external stimuli to help (train) the in virto organoid form the **micro** morphology (connections between neurons).


