# Dataset for *Quantum Delocalization Enables Water Dissociation on Ru(0001)*

This repository provides the LAMMPS input script for molecular dynamics and path-integral molecular dynamics simulations, along with the training and validation datasets used for constructing the machine-learned potential in the following paper:

```bibtex
@article{arXiv.2412.00484,
      title={Quantum Delocalization Enables Water Dissociation on {{Ru}}(0001)}, 
      author={Yu Cao and Jiantao Wang and Mingfeng Liu and Yan Liu and Hui Ma and Cesare Franchini and Yan Sun and Georg Kresse and Xing-Qiu Chen and Peitao Liu},
      year={2024},
      journal={arXiv.2412.00484},
      url={https://arxiv.org/abs/2412.00484}, 
}
```

The training/validation datasets are provided in the extended XYZ format.

## Files

### Training and Validation Data
- **train.xyz**: Training dataset.
- **valid.xyz**: Validation dataset.

### Machine-Learned Potential
- **potential.mtp**: Machine-learned moment tensor potential file with the following atom type mappings:
  - Type 0: Hydrogen (H)
  - Type 1: Oxygen (O)
  - Type 2: Ruthenium (Ru)

### Adsorption Energy
- **Eads**: Directory containing adsorption energies predicted by DFT and MLP for various configurations shown in Figure 1.
  - **Configuration.*.vasp**: Structures of each adsorption configuration corresponding to configuration index in Figure 1.
  - **Eads.dat**: Adsorption energies for each configuration. 

### Molecular Dynamics Simulations
- **MD**: Directory containing initial structures and LAMMPS input scripts for MD simulations at different temperatures:
  - **H2O_md_300K**: MD simulations under 300K.
  - **H2O_md_350K**: MD simulations under 350K.
  - **H2O_md_400K**: MD simulations under 400K.

  Each folder contains:
  - **lammps.in**: LAMMPS input script. 
  - **lat.lmp**: Initial structure for MD simulation.
  - **last.lammpstrj**: Structure snapshot of the last frame of the MD simulation. 

### Path-Integral Molecular Dynamics Simulations
- **PIMD**: Directory containing initial structures and LAMMPS input scripts for PIMD simulations:
  - **D2O_pimd_16_beads_300K**: PIMD simulations under 300K for D2O/Ru(0001) system. 
  - **H2O_pimd_16_beads_300K-{1,2,3}**: PIMD simulations under 300K for H2O/Ru(0001) system, with different random seeds.
  - **H2O_pimd_32_beads_300K**: PIMD simulations under 300K with 32 beads.

  Each folder contains:
  - **lammps.in**: LAMMPS input script. 
  - **lat.lmp**: Initial structure for MD simulation.
  - **last_\*.lammpstrj**: Structure snapshots of the last frame of the PIMD simulation for each bead (16 beads for 16-bead simulations, 32 beads for 32-bead simulations).

## License

This dataset is made available under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/). You are free to share and adapt the material for any purpose, provided you give appropriate credit to the original authors.

## Contact

For any questions or issues regarding this dataset, please contact the corresponding authors of the paper.

---

We hope this dataset will be useful for your research. Thank you for your interest!
