# FULPs-Framework-CA-Application
An application of the FULPs Framework, within the Cellular Automata field of study. Main attempt is to see if FULPs can improve when applied to Conway's Game of Life and then implement adaptive learning, if possible.

# FULPs in Cellular Automata: Adaptive Learning, Recovery, and Signalling in Conway’s Game of Life

This repository contains an experimental implementation of the **Framework of Unified Learning Principles (FULPs)** within a **Conway’s Game of Life (GoL)** cellular automaton environment.

The project explores whether locally adaptive observer cells—equipped with contradiction-aware learning, confidence gating, and neighbour distress signalling—can improve:

* **state prediction accuracy**
* **recovery after environmental perturbation**
* **system stability**
* **emergent spatial coordination**

across repeated simulation runs.

The work progresses through five staged experimental versions, moving from passive observer learning to distributed adaptive signalling, with the goal of testing whether biologically inspired local learning rules can generate meaningful system-level advantages inside a classic CA substrate.

---

## Research Motivation

Traditional cellular automata apply fixed transition rules uniformly across all cells. In contrast, this project investigates whether each cell can act as a local predictive observer, learning the dynamics of its neighbourhood and adapting its behavior based on uncertainty.

The hypothesis is that:

> **Cells that learn from contradiction and adapt based on confidence can improve both local predictive performance and global recovery behavior within a CA environment.**

To test this, FULPs mechanisms are layered incrementally into a Game of Life system:

1. **Local contradiction-aware learning**
2. **Adaptive confidence gating**
3. **Neighbour distress signalling**

Each mechanism is evaluated through controlled perturbation experiments and multi-run statistical comparisons against baseline systems.

---

## Core Framework Concepts

### 1. Contradiction-Aware Learning

Each cell tracks prediction confidence for neighbourhood states using:

* positive similarity
* negative similarity
* contradiction margin

This allows each observer to detect when its expectations no longer match observed outcomes.

### 2. Confidence Gating

Cells with low confidence defer updates, creating an adaptive asynchronous mechanism designed to reduce unstable transitions during perturbations.

### 3. Distress Signalling

Cells broadcast a local scalar “distress” signal based on contradiction strength. Neighbouring cells incorporate this signal when determining their effective gating thresholds, enabling **distributed local coordination**.

---

## Experimental Progression

The repository is organized as an experimental arc:

### **v1 — Observer Learning Baseline**

Introduced FULPs-weighted observer learning and compared it to uniform baseline learning.

**Outcome:**
FULPs improved per-state learning accuracy over baseline.

---

### **v2 — Convergence and Breadth**

Extended the analysis to measure:

* convergence speed
* stable vs unstable state learning
* breadth of coverage

**Outcome:**
FULPs improved convergence and achieved stronger performance in unstable regions.

---

### **v3 — Perturbation Recovery**

Introduced rule perturbations to test recovery under environmental change.

**Outcome:**
FULPs observers recovered significantly faster after perturbation than baseline learners.

---

### **v4 — Confidence-Gated Adaptation**

Added confidence-based update gating to reduce unstable transitions during recovery.

**Outcome:**
Confidence gating improved recovery speed and reduced post-perturbation variability.

---

### **v5 — Distress Signalling**

Added neighbour signalling based on contradiction-derived distress values.

**Outcome:**
Neighbour signalling increased post-perturbation spatial coordination and further improved adaptive recovery behavior.

---

## Key Findings

Across the staged experiments:

* **FULPs observers outperformed baseline learners** in final prediction accuracy.
* **Recovery time after perturbation improved significantly** with adaptive mechanisms.
* **Confidence gating reduced post-perturbation instability.**
* **Neighbour signalling increased spatial coordination**, measured through post-perturbation clustering metrics.

These results suggest that:

> **Local contradiction-aware adaptation can produce measurable system-level advantages in a cellular automaton environment.**

---

## How to Run

### Requirements

Install dependencies:

```bash
pip install numpy scipy pandas matplotlib
```

### Running the Experiments

Open the notebooks in Jupyter:

```bash
jupyter notebook
```

Run the notebooks sequentially:

1. `v1_observer_learning.ipynb`
2. `v2_convergence_breadth.ipynb`
3. `v3_perturbation_recovery.ipynb`
4. `v4_confidence_gating.ipynb`
5. `v5_distress_signalling.ipynb`

Each notebook is self-contained but builds conceptually on the previous version.

---

## Future Work

Potential next steps include:

* tuning signalling strength dynamically
* extending FULPs mechanisms to other CA rule systems
* introducing multi-channel signalling
* exploring adaptive topology changes
* testing transferability to agent-based systems

The broader goal is to investigate whether local contradiction-sensitive learning rules can produce robust emergent adaptation across discrete dynamical systems.

---

## Author

**William Fullerton**
Statistics & Data Science | Computational Systems Research

This repository represents an experimental exploration of adaptive observer architectures in cellular automata, combining concepts from:

* machine learning
* complex systems
* cellular automata
* biologically inspired adaptive computation
