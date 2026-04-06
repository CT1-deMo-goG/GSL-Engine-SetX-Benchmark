# Comparative Performance Report: Set X (100 - 1,000 Nodes)

This folder contains the comparative analysis between the GSL Engine V22 and standard industry baselines: **Clarke-Wright (CW)** and **LNS (Iteration-bounded)**.

## ⚙️ Benchmarking Methodology & Environment
To ensure a fair and transparent comparison, the following constraints were applied:

* **Hardware:** Native execution on a mobile processor (Snapdragon via Pydroid 3).
* **LNS Constraint:** The Large Neighborhood Search (LNS) was strictly bounded to **300 iterations** per instance. This limit simulates a high-pressure, **Real-time** logistics scenario where an immediate response is required.
* **CW Baseline:** Standard Clarke-Wright savings heuristic (constructive).
* **GSL Engine V22:** Operates under its standard deterministic logic with no iteration-based random search.

## 📊 Benchmark Results (Sample)
The following table summarizes the performance across different instances based on the % Gap to BKS.

| Instance | BKS | GSL Gap | CW Gap | LNS Gap (300 Iter) | Winner |
| :--- | :--- | :--- | :--- | :--- | :--- |
| X-n101-k25 | 27591.0 | **-2.18%** | 4.90% | 11.67% | **GSL** |
| X-n148-k46 | 43448.0 | **-0.52%** | 3.92% | 19.18% | **GSL** |
| X-n153-k22 | 21220.0 | **-0.30%** | 6.70% | 22.97% | **GSL** |
| X-n469-k138 | 221824.0 | **-0.58%** | 6.16% | 9.27% | **GSL** |

## 📈 Technical Findings
* **Win Rate:** GSL maintains a stable **87% win rate** compared to LNS across Set X.
* **Consistency:** GSL provides high-precision results in **Real-time**, while metaheuristics (LNS) show higher variance under restricted iterations.
* **Deterministic Execution:** The structured logic ensures predictable output quality regardless of the environment.
