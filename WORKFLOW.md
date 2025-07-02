# Workflow for The Project

1. Begin with unitary matrix mechanics
* Use QuTiP + basic NumPy matrices to replicate your beam splitter, mirror, detector modules.
* Simulate wavefunction evolution through each stage.

2. Visualize tabletop setups
* Use QOptCraft to map component positions.
* Overlay wavefunction amplitudes or probabilities at each optical element in static diagrams using Matplotlib.

3. Wrap with noise + decoherence (optional)
* Transition to Lindblad master equations in QuTiP using built-in solvers or your own RK4 integrator 
* Test randomness and imperfections with SOQCS.

4. Include both PennyLane & Qiskit
* For purely gate-based quantum analogues, you can recreate the same interferometer behavior using qubit circuits in PennyLane and Qiskit.
* Compare their performance and output (state vectors, probability histograms)—great for a portfolio piece.
