# open-science-prize-swap-gate
Improve the fidelity of the SWAP gates between qubits 5 and 6 on the IBM Quantum system ‘ibmq casablanca’ by reducing the infidelity from 2% to 1% with error bars equal to or better than 0.08% using benchmarking techniques described in the Open Science Prize notebook On our IBM Quantum processors, qubits can only interact with neighboring qubits - but several quantum circuits, such as those required for measuring Quantum Volume, frequently require operations between non-neighboring qubits. Quantum computers implement these operations by first using the SWAP gate to bring the quantum states of qubits closer on the chip, and then acting on these qubits with nearest-neighbor quantum gates. IBM Quantum Experience users will use Qiskit Pulse in order to devise SWAP gates of their own, and then characterize the gate’s fidelity, using a Jupyter notebook supplied by IBM Quantum. The goal is to improve the fidelity of the currently implemented SWAP gates. In order to receive access to IBM Quantum System ’ibmq casablanca’, you must demon- strate an understanding of the rigor of the challenge. Choose the challenge you are competing in and briefly de- scribe how you plan to solve that challenge. Confirmation of access will be sent to you via email.

## J. A. Montanez-Barrera and Michael R. von Spakovsky
In our approach, we use the same sequence of pulses from the default SWAP gate, a sequence of three CNOT gates, using a calibration process which is a similar but somewhat different process from that introduced by Kelly et. al. [1]. We use a Random Benchmarking sequence of Clifford gates to calibrate the amplitude of one and two-qubit gates.

The document is organize as follows:

- Amplitude of the Gaussian Pulse Calibration
- Amplitude of the Derivative Gaussian Pulse Calibration
- Amplitude of the Cross Resonance Pulse Calibration
- Amplitude of the rotary echoes in the target qubit calibration
- Testing using the SWAP gate

[1] “Optimal quantum control using randomized benchmarking,” Physical Review Letters, vol. 112, no. 24, pp. 1–5, 2014.
