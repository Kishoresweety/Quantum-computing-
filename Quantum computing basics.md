# 🧑‍💻 Quantum Computing Basics

🔹 1. What is Quantum Computing?

Classical computers → Use bits (0 or 1).

Quantum computers → Use qubits (0, 1, or both at once).

Benefit → Solve problems much faster than classical in some domains.



---

🔹 2. Key Quantum Concepts

1. Qubit (Quantum Bit)

A qubit can be:

|0⟩ (zero)

|1⟩ (one)

Or a superposition of both.



👉 Example: Like a spinning coin = both heads & tails until measured.




---

2. Superposition

Qubit can be in multiple states at once.

Classical bit = either 0 or 1.

Quantum qubit = 0 and 1 at same time.





---

3. Entanglement

Two qubits linked → Changing one affects the other instantly.

Basis of quantum teleportation & fast computation.





---

4. Quantum Gates

Like logic gates in classical computing.

Example:

Hadamard gate (H) → Creates superposition.

CNOT gate → Creates entanglement.






---

5. Measurement

When you observe a qubit → it collapses to 0 or 1.

Example: Until you measure, a qubit can be both 0 and 1.





---

🔹 3. Why Quantum Matters?

Cryptography → Break RSA encryption with Shor’s Algorithm.

Optimization → Solve big problems (logistics, finance).

Drug Discovery → Simulate molecules faster.

AI Acceleration → Speed up training & inference.



---

🔹 4. Example: Quantum Hello World

Using Qiskit (Python library for quantum computing):

from qiskit import QuantumCircuit, Aer, execute

# Create a quantum circuit with 1 qubit
qc = QuantumCircuit(1, 1)

# Apply Hadamard gate -> superposition
qc.h(0)

# Measure qubit
qc.measure(0, 0)

# Run on simulator
backend = Aer.get_backend('qasm_simulator')
job = execute(qc, backend, shots=10)
result = job.result()

print(result.get_counts())

👉 Output may be something like:

{'0': 6, '1': 4}

This shows probability distribution (not fixed like classical).


---

🔹 5. Real-World Example (Simple)

Classical computer → Check 1 key at a time.

Quantum computer → Tries many keys at once (parallel).


That’s why quantum is dangerous for current encryption.


---

🔹 6. Quantum vs Classical

Feature	Classical	Quantum

Unit of data	Bit (0/1)	Qubit (0+1)
Parallelism	Limited	Massive (superposition)
Security	Breakable	Can break encryption
Use cases	General	Optimization, AI, cryptography



---

✅ Summary:

Quantum uses qubits, superposition, entanglement, gates.

Powerful for optimization, cryptography, AI, simulations.

Tools: Qiskit (IBM), Cirq (Google), Braket (AWS).


