# QAOA for Beginners — an interactive lecture

Google Colab Link: [https://github.com/pushpita-c/qaoa-for-beginners/blob/main/qaoa_lecture.ipynb](https://github.com/pushpita-c/qaoa-for-beginners)

A hands-on introduction to the **Quantum Approximate Optimization Algorithm (QAOA)**! You don't need any quantum background**. It takes you from "what is a qubit?" to solving your own optimization problem — and is meant to prepare you for a quantum hackathon.

**Notebook:** `qaoa_lecture.ipynb` (Python + Qiskit, runs on a normal laptop or in Google Colab; no quantum hardware needed)

## What you will learn

| Part | Topic |
|---|---|
| 0 | Quantum computing from zero: qubits, gates, interference, measurement |
| 1 | A hard problem: Max-Cut on a graph |
| 2 | Turning the problem into a Hamiltonian |
| 3 | The QAOA circuit: cost layer + mixer |
| 4 | The p = 1 landscape, running the optimizer, shot noise |
| 5 | More layers, and a smart starting point |
| 6 | **Your own problem:** QUBO → Ising → QAOA toolkit, constraints as penalties |
| 7 | **Hackathon playbook:** project plan, pitfalls checklist, going further |

## How to run

**Google Colab (no install):** open https://colab.research.google.com, choose *File → Upload notebook*, and select `qaoa_lecture.ipynb`.
(Once this repo is public you can also use `https://colab.research.google.com/github/<user>/<repo>/blob/main/qaoa_lecture.ipynb`.)
Run the cells from top to bottom. The first code cell installs anything that is missing.

**Locally:**
```bash
pip install -r requirements.txt
jupyter lab qaoa_lecture.ipynb
```

Tested with Python 3.13 and Qiskit 2.5. The whole notebook runs in about 2 minutes; the sliders need a live Jupyter/Colab session (they do not move on GitHub's static preview).

## Tips

* Run the cells in order; later cells use functions defined earlier.
* **Play with every slider** — that is where the intuition comes from.
* If a plot does not show up in Jupyter, run `%matplotlib inline` once.

## References

* E. Farhi, J. Goldstone, S. Gutmann, *A Quantum Approximate Optimization Algorithm*, arXiv:1411.4028 (2014).
* A. Lucas, *Ising formulations of many NP problems*, arXiv:1302.5843 (2014).
