# GSL Engine
### High-Velocity Deterministic Solver for CVRP
**Logistics Optimization with Operational Focus**

---

## Overview
**GSL Engine** is a proprietary high-performance solver for the Capacitated Vehicle Routing Problem (CVRP). The engine is designed with an operational mindset: delivering fast, stable, and reproducible routing solutions suitable for real-world logistics environments.

Rather than pursuing theoretical optimality at any computational cost, GSL prioritizes:
* **Deterministic behavior**
* **High speed-to-quality ratio**
* **Scalability across large instances**
* **Practical deployment viability**

## Benchmark Validation
The engine was evaluated against the complete **Set X (100 instances)** from CVRPLIB, the standard public benchmark for CVRP research.

### Summary Results
* **Instances Evaluated:** 100 / 100
* **Node Coverage:** 100% (Full Integrity / Zero-Loss)
* **Average Gap vs. Recorded BKS:** 7.42%
* **Average Runtime:** ~1.08 seconds per instance
* **Total Batch Runtime:** ~108 seconds

*Note: All runs were executed in a constrained local runtime environment to simulate realistic deployment conditions.*

## Notable Observations (BKS Challengers)
During evaluation, GSL produced solutions with total distances lower than the BKS values recorded in the benchmark snapshot:

| Instance | GSL Distance | Recorded BKS | Relative Diff |
| :--- | :--- | :--- | :--- |
| **X-n148-k46** | 43,167.85 | 43,448.00 | **-0.64%** |
| **X-n469-k138** | 221,312.75 | 221,824.00 | **-0.23%** |
| **X-n153-k22** | 21,178.91 | 21,220.00 | **-0.19%** |
| **X-n670-k130** | 146,249.90 | 146,332.00 | **-0.06%** |

## Design Philosophy
GSL is built around a **structured deterministic heuristic framework** guided by internal constraint logic. The system does not claim guaranteed global optimality; instead, it targets a balance between solution quality and computational responsiveness, aligning with real-world logistics demands.

## Intellectual Property
The core algorithmic structure and implementation remain **strictly proprietary**. This repository serves as a performance portfolio and validation record.

## Contact
For technical discussions, collaboration, or licensing inquiries:
**Email:** ctsuwan@proton.me

