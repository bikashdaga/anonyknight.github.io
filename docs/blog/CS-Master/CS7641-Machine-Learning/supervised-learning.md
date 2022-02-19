---
title: CS7641-SL
title_full: CS7641 Supervised Learning
description: Machine Learning
tags:
  - OMSCS
  - Machine Learning
---

## Classification vs regression

Discrete labels vs continuous label

## Classification Learning

* **Instances**: (Input vectors of values)
* **Concept**: Function to map input to output. Idea to describe things.
* **Target concept**: actual answer.
* **Hypothesis class**: all possible functions.
* **Sample**: **training set**. Input data with correct labels.
* **Candidate**: concept might be target concept.
* **Testing set**: Should not be the same as Training set.

## Decision Trees

### 20 questions

Ask 20 questions to guess what's in another person's mind?

Each question **further narrow down** the scope.

## Steps

1. Pick best attribute to **split** the data (in binary)
2. Asked question
3. Follow the answer path
4. Go to Step 1 until get an answer.

### Expressiveness

Boolean functions: 

AND

OR

XOR: full truth table.

#### N-OR (Any)

Linear N nodes.

#### N-XOR (Parity)

2**N - 1 nodes.

### ID3

Loop:

* A < - Best attribute
* Assign A as decision attribute for node
* For each value of A, create a descendent of node
* Sort training examples to leaves
* If examples per

### How to find the best attribute?

### Information gain

If it's even, there is no way to guess what's the possibility of the result. Information is the maximum. If it's 100% sure, then information is none.

#### Entropy

A measure of randomness.
$$
Gain = Entrosy(S) - \Sigma \dfrac{|Sv|}{|S|} Entropy(S_v)
$$
The goal is maximize entropy gain.

### Bias

Inductive Bias

Restriction Bias

Preference Bias

## 
