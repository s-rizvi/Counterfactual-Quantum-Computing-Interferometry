# 🛠️ Workflow for the C.Q.C.I. Project

This project is structured in four progressive stages, moving from idealized unitary simulations to hybrid circuit-based implementations and decoherence modeling.

---

## 1️⃣ Begin with Unitary Matrix Mechanics

- Use **QuTiP** along with **NumPy** to simulate the core quantum optical components:
  - Beam splitters
  - Mirrors
  - Phase shifters
  - Detectors

- Represent quantum states as vectors and operators as matrices.
- Simulate **wavefunction evolution step-by-step** through each interferometer configuration.

---

## 2️⃣ Visualize Tabletop Setups

- Use **QOptCraft** or manual schematics to define optical layouts.
- Recreate experimental configurations as labeled 2D diagrams.
- Use **Matplotlib** to generate static images:
  - Optical components
  - Light paths
  - Wavefunction amplitudes/probabilities at key nodes
  - Final detector probabilities

*(No animations—only still diagrams designed for clarity and pedagogy.)*

---

## 3️⃣ Wrap with Noise and Decoherence (Optional)

- Transition to **Lindblad master equations** in QuTiP for open system simulations.
- Use QuTiP's solvers or implement your own **Runge-Kutta 4th Order (RK4)** integrator for more control.
- Explore imperfections via frameworks like **SOQCS**:
  - Lossy optics
  - Detector inefficiencies
  - Misalignment jitter

---

## 4️⃣ Include Both PennyLane & Qiskit

- Recreate the interferometry logic as **quantum circuits** using qubits:
  - Use **PennyLane** and **Qiskit** to model gate-based analogues of beam splitters and phase shifters.
  - Build and visualize logic-gate equivalents to the same experiments.

- Compare results from matrix mechanics and circuit-based quantum simulation:
  - State vectors
  - Probabilities
  - Efficiency and performance (especially on low-end hardware)

---

This staged approach ensures a pedagogical ramp-up from simple to complex, while showcasing a variety of quantum frameworks within a consistent experimental structure.
