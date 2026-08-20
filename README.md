# GNINA-Beginner-Docking

A minimalist, beginner-friendly pipeline for performing molecular docking using **GNINA** (a deep learning-based extension of AutoDock Vina) and analyzing both empirical binding affinities and CNN confidence scores.

## 🧬 Project Overview
This repository automates a basic protein-ligand docking workflow. It demonstrates how to run GNINA, generate binding poses, and interpret:
1. **Vina Affinity (kcal/mol)**: Traditional physics-based scoring.
2. **CNN Score / CNN Pose**: Deep learning-based scoring (ranging from 0 to 1) indicating structural plausibility.

---

## 📂 Repository Structure
```text
GNINA-Beginner-Docking/
├── input/
│   ├── receptor.pdbqt      # Prepared target protein structure
│   └── ligand.pdbqt        # Prepared ligand structure
├── output/                 # Generated docked poses and logs
├── run_docking.sh          # Automation script to execute GNINA
└── README.md               # Project documentation
