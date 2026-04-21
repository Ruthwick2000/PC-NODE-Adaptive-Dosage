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
