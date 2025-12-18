# HeatFlux_MLP_LAMMPS

This is an implementation for calculating heat flux using Machine Learning Potentials (MLPs) within LAMMPS (Large-scale Atomic/Molecular Massively Parallel Simulator). This implementation enables the accurate calculation of per-atom stress with machine learning potentials.

I have personally tested and confirmed to work for **LAMMPS ver(29 Aug 2024)**.

---

## File Descriptions

* **Si.mtp**: A trained Moment Tensor Potential file for Silicon (Si).
* **Cu.mtp**: A trained Moment Tensor Potential file for Copper (Cu).
* **pair.cpp, pair.h, pair_*.cpp**: Modified LAMMPS source files for the accurate implementation of per-atom stress for machine learning potentials.
* **README.md**: This file.

---

## How to Use

To use this implementation with LAMMPS, please follow the steps below.

1.  **Copy Source Files**
    Copy the `pair.cpp` and `pair.h` files into the `src` directory of your LAMMPS installation. Moreover, copy the `pair_*.cpp` files into each MLP package directories. This will overwrite the existing files, so please back up the original files if necessary.

2.  **Rebuild LAMMPS**
    After copying the files, rebuild your LAMMPS executable. This will apply the changes to the simulator.


