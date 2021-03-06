# open-science-prize-swap-gate
Improve the fidelity of the SWAP gates between qubits 5 and 6 on the IBM Quantum system ‘ibmq casablanca’ by reducing the infidelity from 2% to 1% with error bars equal to or better than 0.08% using benchmarking techniques described in the Open Science Prize notebook On our IBM Quantum processors, qubits can only interact with neighboring qubits - but several quantum circuits, such as those required for measuring Quantum Volume, frequently require operations between non-neighboring qubits. Quantum computers implement these operations by first using the SWAP gate to bring the quantum states of qubits closer on the chip, and then acting on these qubits with nearest-neighbor quantum gates. IBM Quantum Experience users will use Qiskit Pulse in order to devise SWAP gates of their own, and then characterize the gate’s fidelity, using a Jupyter notebook supplied by IBM Quantum. The goal is to improve the fidelity of the currently implemented SWAP gates. In order to receive access to IBM Quantum System ’ibmq casablanca’, you must demon- strate an understanding of the rigor of the challenge. Choose the challenge you are competing in and briefly de- scribe how you plan to solve that challenge. Confirmation of access will be sent to you via email.

## J. A. Montanez-Barrera and Michael R. von Spakovsky
In our approach, we use the same sequence of pulses from the default SWAP gate, a sequence of three CNOT gates and a pair of Hadamard gates in both qubits. What is different in our approach is calibration process. Instead of using a sequence of predefined gates, we use a set of random Clifford gates, which is a similar but somewhat different process from that introduced by Kelly _et. al_. [1], since we use a selective random benchmarking process for adjusting the different parameters. We use a set of random Clifford gates and vary the amplitude of the DRAG pulse in single qubits, when we get closer to the better amplitude, we increment the number of Clifford gates. In the future, we plan to use the same process of calibration for the CR amplitude and the rotary echoes of the CNOT gates.

The document is organize as follows:
- Amplitude of the Gaussian Pulse Calibration
- Amplitude of the Derivative Gaussian Pulse Calibration
- Testing using the SWAP gate 

[1] “Optimal quantum control using randomized benchmarking,” Physical Review Letters, vol. 112, no. 24, pp. 1–5, 2014.


## Results
![res_mine](https://user-images.githubusercontent.com/11268357/115100146-7368da80-9f00-11eb-9972-48f26a6fc3b9.png)
