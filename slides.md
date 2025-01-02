---
marp: true
theme: default
header: Brain Sciences and Brain Disorders 2024 Fall
footer: "Group 10: 刘思昀、虞果、唐林峥"
paginate: true
math: katex
style: |
  section::after {
    content: attr(data-marpit-pagination) '/' attr(data-marpit-pagination-total);
  }
---

# Intelligent Brain Organoid

Developing Functional Neural Networks in Brain Organoids with FEP

---

# Catalog

1. ### Introduction
1. ### Background
1. ### Proposed Methodology
1. ### One Specific Design

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

- Physically hard to reconstruct.

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

- Functionally: Actively **"train"** the organoid, giving brain organoids complete stimuli like a real brain will receive.

![bg right:55% fit 95%](image/slides/demo-dishbarin.png)

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

<div>

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

---

# One Specific Design

### A more effective depression model


---

# One Specific Design
## Why Depression Modeling?

- Depression involves complex neural and biochemical disruptions.

- There is still controversy surrounding animal models of depression.

![bg contain right 90%](image/slides/depression-model.png)

---

# One Specific Design
## Goal

- Create a functional neural network model to simulate depression-related features.

- Combine DishBrain’s electrical training with external chemical stimuli.

---

# One Specific Design
## Experimental Design

- Neuronal Culture

  - Culture hiPSC-derived neurons into Hippocampus-like region directly on MEA Chips.

<div style="margin-left: 200px">

![](image/slides/to-hippocampus.png)

</div>

---

# One Specific Design
## Experimental Design

- External Continual Stimuli

  - Chemical: Corticosterone, IL-6, TNF-α.

  - Impairs neural plasticity and reduces network activity.

  - Alters synaptic connectivity.

  - DishBrain-style training including **electical stimuli** and **chemical stimuli**.

---

# One Specific Design
## Application

- Innovative approach to model depression mechanisms.

- Drug screening.

- Understanding network-level changes in mental health disorders.


---

# References
- Friston, K. The free-energy principle: a unified brain theory?. Nat Rev Neurosci 11, 127–138 (2010). https://doi.org/10.1038/nrn2787

- In vitro neurons learn and exhibit sentience when embodied in a simulated game-world; Kagan, Brett J. et al.; Neuron, Volume 110, Issue 23, 3952 - 3969.e8

- Kim SH, Chang MY. Application of Human Brain Organoids-Opportunities and Challenges in Modeling Human Brain Development and Neurodevelopmental Diseases. Int J Mol Sci. 2023 Aug 7;24(15):12528. doi: 10.3390/ijms241512528. PMID: 37569905; PMCID: PMC10420018.
