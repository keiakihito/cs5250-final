# Selective Quantum Advantage: A Classical vs Quantum Search Comparison

This project demonstrates the concept of **selective quantum advantage** through code-based simulations using Qiskit.

We compare:
- Classical linear search: O(N)
- Grover's quantum search algorithm: O(√N)
- Show a trivial task where quantum computing provides no benefit (even/odd check)

---

## Demo Video

You can watch the full walkthrough here:  
[https://youtu.be/ND-HLmCc2ig](https://youtu.be/ND-HLmCc2ig)

---

## What's in the Notebook?

The notebook is structured into three key sections:

### 1. Classical Linear Search

We measure the average runtime of classical linear search over a list of increasing sizes — from 64 to 2048 elements.  
This gives us a clear O(N) performance baseline.

### 2. Grover's Algorithm (Quantum Search)

We simulate Grover's algorithm for `n` = 2 to 6 qubits (which means N = 4 to 64).  
Although Grover provides **quadratic speedup in theory**, the actual simulation on a classical CPU is **slower** due to matrix computation overhead.  
Still, we observe its favorable scaling characteristics.

### 3. Even/Odd Check: Quantum vs Classical

We compare how a classical `n % 2` operation vastly outperforms a full quantum circuit that does the same thing.  
This shows that **quantum computing is not universally better** — it's best suited for specific problem types.

---

## Key Takeaways

> Quantum computing is not a generalist.  
> It is a **specialist**, offering real advantages only in carefully selected problem domains like unstructured search, optimization, and quantum simulation.

---

## Tech Stack

- Python 3.10
- Qiskit 2.0.1 (via conda-forge)
- Jupyter Notebook
- matplotlib

---