# 1D Phase-Field Simulation of Dealloying in a Ternary System

This repository contains a Jupyter Notebook implementation of a 1D phase-field model to simulate the dealloying process in a ternary (A-B-C) system. The model is based on the Cahn-Hilliard and Allen-Cahn equations to simulate the evolution of concentration and phase fields.

## 📜 Description

Dealloying is a corrosion process where specific elements are selectively removed from an alloy, resulting in a nanoporous structure. This simulation employs a phase-field method, a powerful computational technique for modeling microstructural evolution. While simplified to one dimension, this model provides key insights into the fundamental physics of the dealloying process.

The code is presented in a Jupyter Notebook to allow for interactive execution and easy visualization of the results.

## 💻 How to Run


1.  **Install dependencies:**
    Make sure you have Python installed. Then, install the required libraries using pip:
    ```bash
    pip install -r requirements.txt
    ```

4.  **Open and run the notebook:**
    Click on the `dealloying_1D.ipynb` file to open it. You can then run the cells sequentially to execute the simulation and see the animated results directly within the notebook.

## 📈 Results

The simulation generates an animation that visualizes the evolution of the concentration profiles for the three components (A, B, and C) and the phase field over time. This provides a clear illustration of pore formation and the redistribution of the remaining elements during dealloying.


---
![Dealloying Simulation GIF](phasefield_concentration_evolution.gif)
---

### Explanation of the Results

The animation displays the concentration profiles of the three components (A, B, and C) alongside the phase-field variable ($\phi$) across the 1D domain.

- **Initial State:** The simulation begins with a nearly homogeneous mixture of the three components in a solid phase ($\phi \approx 1$).

- **Phase Separation:** Over time, the system undergoes spinodal decomposition. The concentration profiles begin to fluctuate, showing the separation of the alloy into distinct regions enriched in different components. This is driven by the chemical potential gradients and the system's tendency to minimize its free energy.

- **Dealloying and Pore Formation:** As the simulation progresses, the less noble elements are selectively removed (simulated by their diffusion and phase separation), leading to the formation of pores. These porous regions are identified where the phase-field variable ($\phi$) approaches zero, representing a transition from the solid alloy to a void or liquid-filled phase.

- **Enrichment of Noble Components:** Concurrently, the regions that remain solid become enriched in the more noble components of the alloy, which are stable under the simulated conditions. The final structure consists of a nanoporous material, which is the characteristic outcome of the dealloying process.

This simulation effectively captures the fundamental dynamics of dealloying, providing a visual representation of how a solid alloy evolves into a complex porous structure.


