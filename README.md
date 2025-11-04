# CSS-PAULI-ERROR-JurgenM

# CSS Code under Random Pauli Error

This project simulates a quantum Hamming CSS code [[15,7,3]] under a random Pauli error channel.
The self-dual [[15,7,3]] code with H_X = H_Z given by the parity-check matrix below:
\[
H_X = H_Z =
\begin{pmatrix}
0&0&0&0&0&0&0&1&1&1&1&1&1&1&1\\
0&0&0&1&1&1&1&0&0&0&0&1&1&1&1\\
0&1&1&0&0&1&1&0&0&1&1&0&0&1&1\\
1&0&1&0&1&0&1&0&1&0&1&0&1&0&1
\end{pmatrix}.
\]
## Files

- `css_code.py`: Implements the code, noise, syndrome measurement, and recovery.
- `experiment.py`: Runs multiple trials over a sweep of error probabilities.
- `results_css.npz`: Saved results from experiment.
- `success_vs_p.png`: Plot of success probability vs error probability.

## Running the Experiment

**


## Results

The success probability correct logical zero outcome is plotted as a function of error rate `p`.

## Notes

- The recovery operation is a placeholder; accuracy improves with a real decoder.
- Only Clifford gates, measurements, and classically controlled Pauli operations are used, except for state preparation.
- Total qubits required = 15 (physical) + 8 (ancilla) = 23.
- For p = 0.02, success rate: 93%
