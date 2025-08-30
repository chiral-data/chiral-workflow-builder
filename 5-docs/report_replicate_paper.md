# Replication Report: [Paper Title]

**Original Paper:** [Full citation with DOI/link]  
**Authors:** [Names]  
**Replication Author:** [Your name]  
**Date:** [YYYY-MM-DD]

---

## 1. Objective

from project plan

---

## 2. Computational Environment

from project plan

---

## 3. Schedule

| Task               | Description                                       | Estimated Time (hours) | Actual Time (hours)  |
| ------------------ | ------------------------------------------------- | ---------------------- | -------------------- |
| Environment setup  | Install software, prepare environment             | [e.g., 3h]             | [e.g., 3h]           |
| System preparation | Structure download, protonation, parameterization | [e.g., 5h]             | [e.g., 3h]           |
| Minimization       | Energy minimization of system                     | [e.g., 1h]             | [e.g., 3h]           |
| Equilibration      | NVT + NPT equilibration runs                      | [e.g., 10h]            | [e.g., 3h]           |
| Production MD      | Full trajectory (e.g., 100 ns × 3 replicas)       | [e.g., 200h]           | [e.g., 3h]           |
| QM calculations    | Single-point / optimization                       | [e.g., 50h]            | [e.g., 3h]           |
| Analysis           | RMSD, free energy, statistics                     | [e.g., 6h]             | [e.g., 3h]           |
| Report writing     | Documentation and visualization                   | [e.g., 5h]             | [e.g., 3h]           |
| **Total**          |                                                   | **[sum of above] h**   | **[sum of above] h** |

---

## 4. System Preparation

- **Source of structures**: [PDB ID, PubChem ID, provided SI, etc.]
- **Protonation/tautomers**: [Method/tool used, pH condition]
- **Ligand parameterization**: [Force field, charges, tool (GAFF, CGenFF, OpenFF)]
- **Protein force field**: [AMBER ff14SB, CHARMM36, etc.]
- **Solvation**: [Water model, box type and size, ion concentration]
- **Special constraints**: [Disulfide bonds, restraints, mutations]

---

## 5. Computational Protocol

### 5.1 Minimization & Equilibration

- Minimization steps: [# of steps, convergence criteria]
- Equilibration ensembles: [NVT, NPT, thermostat/barostat]
- Time step and cutoff: [fs, Å]
- Duration: [ns]

### 5.2 Production Simulation / Quantum Calculations

- Molecular dynamics:
  - Length of trajectory: [X ns per replica]
  - Replicates: [#]
  - Random seed policy: [fixed/random]
- Quantum mechanics:
  - Method/functional: [HF, DFT, MP2, etc.]
  - Basis set: [6-31G*, def2-SVP, etc.]
  - Convergence criteria: [energy, gradients]

### 5.3 Free Energy / Binding Affinity Calculations

- Method: [MM/PBSA, TI, FEP, metadynamics]
- Protocol details: [window spacing, lambda schedule, sampling time]

---

## 6. Analysis

- **Metrics computed**:
  - RMSD, RMSF, H-bonds, energy components, cluster analysis, free energies.
- **Statistical treatment**:
  - Averaging method, error bars, bootstrap/block averaging.
- **Plots and figures**:
  - Attach energy/time plots, histograms, convergence plots.

---

## 7. Results

- **Original reported values**:
  - Binding free energy: [value ± error]
  - Structural metrics: [RMSD ranges, conformations]
  - QM results: [relative energies, HOMO-LUMO gaps, etc.]

- **Replication values**:
  - [Your results, with uncertainties and notes]

- **Comparison**:
  - Quantitative deviations (absolute/relative error).
  - Qualitative agreement (same binding pose, same trends, etc.).

---

## 8. Discussion

- **Possible reasons for discrepancies**:
  - Random fluctuations / insufficient sampling
  - Hidden details in original methods
  - Different software versions
  - Force field or basis set updates

- **Reproducibility assessment**:
  - Fully reproducible, partially reproducible, or not reproducible.
- **Suggestions for improvement**:
  - More explicit methodological details in original paper
  - Sharing of input/output files

---

## 9. Conclusion

- Summary of replication success/failure.
- Scientific implications (does it confirm the original claims?).
- Next steps (e.g., extend simulation, alternative methods).

---

## 10. Data & Code Availability

- **Input files repository**: [GitHub/Zenodo link]
- **Analysis scripts**: [Link or description]
- **Environment specification**: [environment.yml / Dockerfile attached]

---

## Appendix

- Full parameter files (MDP, Gaussian input, etc.).
- Additional plots or raw data.
