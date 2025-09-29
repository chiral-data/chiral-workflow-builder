# Replication Planning: [Paper Title]

**Original Paper:** [Full citation with DOI/link]  
**Authors:** [Names]  
**Replication Author:** [Your name]  
**Date:** [YYYY-MM-DD]

---

## 1. Objective

- What is being replicated?
- Specific goals (e.g., reproduce free energy calculation, confirm binding mode stability, reproduce DFT energies).
- Scope and limitations (e.g., partial replication, only MD but not QM part).

---

## 2. Computational Environment

- **Hardware**: [CPU/GPU, cores, memory, cluster/cloud info]
- **Operating System**: [Linux/Mac/Windows, version]
- **Software stack**:
  - Molecular modeling: [GROMACS 2023.1, AMBER 22, etc.]
  - Quantum chemistry: [Gaussian16, ORCA 5.0, etc.]
  - Preprocessing: [OpenEye Spruce, RDKit, etc.]
  - Analysis tools: [MDAnalysis, PyEMMA, VMD]
- **Environment management**: [Conda environment, Docker/Singularity image, module system]

---

## 3. Schedule (Estimated Wallclock Time)

| Task               | Description                                       | Estimated Time (hours) |
| ------------------ | ------------------------------------------------- | ---------------------- |
| Environment setup  | Install software, prepare environment             | [e.g., 3h]             |
| System preparation | Structure download, protonation, parameterization | [e.g., 5h]             |
| Minimization       | Energy minimization of system                     | [e.g., 1h]             |
| Equilibration      | NVT + NPT equilibration runs                      | [e.g., 10h]            |
| Production MD      | Full trajectory (e.g., 100 ns × 3 replicas)       | [e.g., 200h]           |
| QM calculations    | Single-point / optimization                       | [e.g., 50h]            |
| Analysis           | RMSD, free energy, statistics                     | [e.g., 6h]             |
| Report writing     | Documentation and visualization                   | [e.g., 5h]             |
| **Total**          |                                                   | **[sum of above] h**   |
