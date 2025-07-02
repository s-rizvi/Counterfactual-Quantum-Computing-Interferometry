# 🛠️ Workflow for the C.Q.C.I. Project

This project is structured in four progressive stages, moving from idealized unitary simulations to hybrid circuit-based implementations and decoherence modeling.

---

## 1️⃣ Begin with Unitary Matrix Mechanics

Before we do anything, let's create a filesystem structure that includes all modules necessary for our project to succeed.

cqci_project/
├── simulator/
│   ├── __init__.py
│   ├── beam_splitter.py
│   ├── mirror.py
│   ├── detector.py
│   ├── interferometer.py
│   └── utils.py
├── visuals/
│   ├── __init__.py
│   ├── diagram.py
│   └── plotting.py
├── circuithub/
│   ├── __init__.py
│   ├── qiskit_module.py
│   └── pennylane_module.py
├── decoherence/
│   ├── __init__.py
│   ├── lindblad_solver.py
│   └── noise_models.py
├── examples/
│   ├── __init__.py
│   ├── mzi_example.py
│   └── quantum_eraser.py
└── tests/
    ├── __init__.py
    └── test_interferometer.py

Step 1: The project is based on the simulator module, so let's start building our interferometer simulator, starting with beam_splitter.py, mirror.py, detector.py, and interferometer.py. Then we put miscellaneous functions in utils.py and set up __init__.py.

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
