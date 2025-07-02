# Counterfactual Quantum Computing Interferometry (C.Q.C.I.)

> A visual and programmable testbed for simulating and understanding quantum interferometry using matrix mechanics, with support for PennyLane and Qiskit.

---

## 🎯 Project Purpose

**Counterfactual Quantum Computing Interferometry** is a software-only simulation framework for recreating quantum interferometry experiments — including Mach-Zehnder setups, delayed choice erasers, and counterfactual logic gates — using ideal matrix-based mechanics.

This project serves **three purposes**:

- 📚 **Teaching Tool**: Help students and curious minds explore quantum mechanics through optics-based visualizations and experiments.
- 🔬 **Experimental Sandbox**: Test configurations and quantum logic using software simulations before moving to physical implementation.
- 💼 **Portfolio Showcase**: Demonstrate the intersection of physics, data science, and visualization through clean code and rich output.

---

## 🔧 Key Features

- ✅ Simulation of ideal quantum optical components:
  - Beam splitters
  - Mirrors
  - Phase shifters
  - Detectors
  - Polarizers
- 🧮 Unitary matrix mechanics powered by **NumPy** and **QuTiP**
- 🖼️ Static visualizations of "tabletop" optical setups
  - Diagrams label each component, wavefunction amplitudes, and detector probabilities
- 🧠 Support for **delayed-choice experiments** and **counterfactual setups**
- 🔌 Optional Qiskit and PennyLane modules for qubit-based analogues
- 🧊 Roadmap includes support for **decoherence modeling** using Lindblad master equations

---

## 🖥️ Visual Example (Planned)

> 📷 When a full interferometer setup is run, the program will generate a labeled diagram showing:
> - Laser source and beam path
> - Each optical component (BS, M, D, P, etc.)
> - Evolving wavefunction amplitudes at each node
> - Final detector probabilities

*(No animations — just clear snapshots suitable for educational or experimental use.)*

---

## 📂 Repository Structure

| Folder/File                          | Description                                                                                                                   |
| ------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------- |
| [`README.md`](./README.md)           | This file — a guide to the project and its structure.                                                                         |
| [`BACKGROUND.pdf`](./BACKGROUND.pdf) | 10 slides covering the necessary background for understanding the physics behind this project  |

---

## 🗂️ Planned Project Structure

```plaintext
c.q.c.i./
├── simulator/        # Core matrix operations & optical logic
├── visuals/          # Tabletop diagram generation
├── circuithub/       # PennyLane & Qiskit implementations
├── decoherence/      # Lindblad models & noise simulations
├── examples/         # Walkthroughs of specific setups (e.g., MZI, quantum eraser)
├── tests/            # Unit tests
└── README.md
```

---

## ⚙️ Installation

```bash
git clone https://github.com/yourusername/counterfactual-interferometry.git
cd counterfactual-interferometry
pip install -r requirements.txt
```

**Dependencies (in progress):**
- Python 3.9+
- NumPy
- QuTiP
- Matplotlib
- PennyLane
- Qiskit

---

## 👤 Author

Developed by **Noor Rizvi** as part of a data science portfolio.  
Feel free to reach out with questions or ideas.

---

## 📜 License

This project is licensed under the **MIT License**.  
Feel free to use, modify, or adapt with attribution.

---

## 🤝 Contributing

> Contributions welcome once the base framework is complete.
> If you're interested in helping visualize interferometers or implement new setups, feel free to open an issue.

---

## 📌 TODO Roadmap

- [ ] Basic interferometer class (ideal, unitary)
- [ ] Tabletop diagram generator
- [ ] Sample experiments (e.g., quantum bomb tester)
- [ ] PennyLane/Qiskit modules
- [ ] Add noise/decoherence models
- [ ] Advanced circuit visualizer

---

## 🧠 Conceptual Inspirations

- Elitzur–Vaidman Bomb Tester  
- Wheeler’s Delayed Choice Experiment  
- Quantum Eraser Experiments  
- Dirac’s *Principles of Quantum Mechanics*

---

## 🌐 Keywords

`quantum mechanics` `interferometry` `counterfactual computing` `matrix mechanics` `PennyLane` `Qiskit` `QuTiP` `data science` `optics` `simulation`

---
