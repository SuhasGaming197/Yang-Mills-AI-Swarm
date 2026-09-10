# Yang-Mills AI Swarm Orchestrator

This repository contains the prototype for a multi-agent AI orchestrator designed to assist in the formal verification of numerical bounds in computational physics, specifically targeting the **Yang-Mills Mass Gap** (a Clay Millennium Prize problem) and the parameter space for **Leptogenesis**.

The system leverages the **Google Antigravity SDK** to deploy a hierarchy of AI agents (Hypothesis Generators and Verification Agents) to write, execute, and mathematically cross-check Lattice Gauge Theory simulations.

## Project Architecture

The swarm architecture operates in three tiers:
1. **The Lead Theorist (Orchestrator):** Manages the swarm, assigns topological sectors to hypothesis agents, and compiles the final proof document.
2. **Hypothesis Agents:** Autonomous agents that explore specific lattice boundaries (e.g., Weak Coupling limits, Topological Freezing) and generate Python-based numerical scripts (MCMC samplers) to test their hypotheses.
3. **Verification Agents:** Rigorous peer-review agents that cross-check the generated proofs against known lattice constraints to prevent mathematical hallucinations.

## Core Implementations

The project currently contains two functional numerical foundations:
*   **Lattice Gauge Theory MCMC:** A Metropolis-Hastings sampler for 2D SU(2) gauge fields, utilized to extract the scaling curve of the average plaquette energy and demonstrate asymptotic freedom in the weak-coupling limit ($\beta \to \infty$).
*   **Leptogenesis QKE Solver:** A parallelized implicit Radau integrator that solves stiff Quantum Kinetic Equations to map the viable parameter space ($M_1, K$) for dynamically generating the universe's baryon asymmetry.

## Technologies Used
*   **AI / Multi-Agent Systems:** Google Antigravity SDK, Python `asyncio`
*   **Scientific Computing:** NumPy, SciPy (`solve_ivp`), Matplotlib
*   **High-Performance Computing (Target):** MPI/GPU optimization for PARAM Supercomputing Clusters

## Included Files
*   `swarm_orchestrator.py`: The main asynchronous multi-agent deployment script.
*   `scientific_journal_submission.md`: The formal mathematical write-up and computational analysis of the generated results, including contour mapping and lattice scaling curves.

---
*Note: This repository is actively maintained as an independent research prototype for exploring the intersection of Large Language Models and non-perturbative physics.*
