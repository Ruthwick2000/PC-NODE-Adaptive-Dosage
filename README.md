# PC-NODE-Adaptive-Dosage
hysics-Constrained Neural ODE for Environment-Adaptive Drug Dosage — DIAT Pune M.Tech 2026
cat > ~/PC-NODE-Adaptive-Dosage/README.md << 'EOF'
# PC-NODE: Physics-Constrained Neural ODE for Adaptive Drug Dosage

**Author:** Sirangi Ruthwick (Roll No. 24-14-10)
**Supervisor:** Dr. Odelu Ojjela
**Institute:** Defence Institute of Advanced Technology (DIAT), Pune
**Programme:** M.Tech Modelling & Simulation | 2024–2026

---

## Overview

RAG-PCNODE is a Retrieval-Augmented Physics-Constrained Neural Ordinary
Differential Equation that adjusts drug dosage in real time based on:
- Altitude (CYP3A4 enzyme suppression — Zhu et al. 2022)
- Temperature (Renal perfusion reduction — ICMR 2024)
- CYP3A4 Pharmacogenomics (PharmGKB)
- Clinical comorbidities

**Key result:** For an Amarnath pilgrim at 3,888 m with CYP3A4 Poor
Metaboliser genotype, the model recommends 9.9 mg [95% CI: 7.8–12.0 mg]
versus the standard 30 mg — a 67% reduction preventing drug toxicity.

---

## Repository Structure

---

## Key Results

| Metric | RAG-PCNODE | Trans-PK 2026 (extreme) | Classical PK |
|--------|-----------|--------------------------|--------------|
| R²     | 0.9816    | 0.741 ↓                  | 0.871        |
| RMSE   | 3.61 mg/L | 8.90 mg/L ↑              | 8.40 mg/L    |
| Mass-balance violation | <0.1% | 14.8% | 0% |
| Environmental adaptation | Yes | No | No |
| Bayesian CI | Yes | No | No |

---

## How to Run

### Julia (v4 — recommended)
```julia
# Open julia_notebook/pc_node_v4_notebook.jl in Jupyter
# Run cells in order: Cell 1 → Cell 13
```

### Python (v3)
```bash
conda activate pcnode
cd python_code
python pc_node_adaptive_dosage.py
```

---

## Citations

- Zhu et al. (2022). CYP3A4 altitude suppression. *Pharmaceuticals*
- ICMR (2024). Heat stress renal injury. *ICMR Technical Report*
- Gupta & Sharma (2026). Trans-PK. *IEEE Trans. Biomed. Eng.*
- Daglarli (2026). XAI-RAG dosage. *IEEE Access*
EOF
