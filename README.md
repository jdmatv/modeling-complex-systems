# modeling-complex-systems

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

This repository contains notebooks and models developed for the Pardee RAND Graduate School Course 479: Modeling Complex Systems for Policy Analysis.

## Course Description

The course is about policy analysis for social systems in which modeling must deal with both rational-analytic considerations and the messy, wicked, and complex considerations that involve disagreements about values, perspectives, estimates, and even facts. The course teaches good practices for cause-effect modeling for policy analysis, including modeling of complex adaptive systems. It includes hands-on experience with analytic (e.g., formula-based), system dynamic, agent-based, qualitative, and portfolio-analysis models. It discusses relationships to human exercises.

## Overview of Models and Notebooks

The projects in this repository demonstrate several key paradigms in modeling complex systems, using R for system dynamics and analytical models, and NetLogo for agent-based simulations.

### System Dynamics Models (R)

These models use systems of differential equations to capture the aggregate behavior of populations over time.

-   **Replicator Dynamics (`Replicator Dynamics.Rmd`)**: Implements the Replicator Equation from evolutionary game theory to model the evolution of strategies in a population. The notebook analyzes the dynamics of Rock-Paper-Scissors and the Hawk-Dove game, visualizing outcomes on a simplex plot.
-   **Lotka-Volterra Model (`Lotka-Volterra.Rmd`)**: A classic predator-prey model is implemented to explore population cycles. The analysis includes phase-plane plots, the calculation of nullclines, and linear stability analysis via the Jacobian matrix to identify fixed points and their stability.

### Agent-Based Models (NetLogo)

These models simulate the actions and interactions of autonomous agents to observe emergent patterns at the system level.

-   **Wolf Sheep Predation (`Wolf Sheep Predation.nlogo`)**: A foundational agent-based model simulating a predator-prey ecosystem. It demonstrates how local interactions and individual rules (energy, reproduction) for wolves and sheep lead to emergent population-level cycles.
-   **Schelling's Segregation and Gerrymandering (`Segregation-Gerrymandering.nlogo`)**: Extends Thomas Schelling's classic segregation model. Agents move based on a preference for similar neighbors, leading to large-scale segregation. This model adds a layer of political districting to calculate and track the "Efficiency Gap," a measure of gerrymandering, as an emergent property.
-   **Kuramoto Model of Synchronization (`Kuramoto.nlogo`)**: A model of coupled oscillators where each agent adjusts its phase based on its neighbors. It demonstrates how simple local interactions can lead to spontaneous global synchronization, a key feature of many complex systems.
-   **Kuramoto-El Farol Hybrid (`Kuramoto-El Farol hybrid.nlogo`)**: A hybrid model that combines the synchronization dynamics of the Kuramoto model with agent-based decision-making strategies, exploring the interplay between individual choice and collective behavior.

### Analytical & Information-Theoretic Models (R)

This notebook connects system dynamics to concepts from information theory.

-   **Schelling's Model and Entropy (`Schelling's Model, Entropy and Gerrymandering.Rmd`)**: Analyzes a small-scale version of Schelling's model to analytically compute all possible microstates. It identifies which configurations are stable and calculates the system's Shannon Entropy, providing a quantitative measure of the reduction in uncertainty as the system self-organizes.

## Key Concepts and Paradigms

-   **System Dynamics**: Modeling system-wide feedback loops and stocks-and-flows using differential equations.
-   **Agent-Based Modeling (ABM)**: Simulating bottom-up interactions of heterogeneous agents.
-   **Complex Adaptive Systems**: Exploring systems where agents learn and adapt their strategies over time.
-   **Evolutionary Game Theory**: Analyzing the evolution of strategies in a population (e.g., Hawk-Dove).
-   **Emergence**: Observing how macro-level patterns (e.g., segregation, synchronization) arise from micro-level rules.
-   **Stability Analysis**: Identifying system equilibria and their stability using mathematical tools like Jacobians and eigenvalues.
-   **Information Theory**: Applying concepts like Shannon's Entropy to quantify order and self-organization.
-   **Policy-Relevant Metrics**: Developing quantitative measures to assess policy outcomes, such as the Efficiency Gap in gerrymandering.

## Software and Tools

-   **R**: Used for implementing system dynamics models, performing mathematical analysis, and data visualization.
    -   *Key Packages*: `deSolve`, `dplyr`, `ggplot2`, `rootSolve`.
-   **NetLogo**: Used for building and exploring agent-based models of complex adaptive systems.

## Usage

-   **R Markdown files (`.Rmd`)**: Can be opened and run in RStudio. Ensure you have the required packages listed in the `setup` chunk of each file.
-   **NetLogo models (`.nlogo`)**: Can be opened and run using the NetLogo application (version 6.4.0 or compatible).

## License

This project is licensed under the MIT License.
