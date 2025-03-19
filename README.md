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

- **train.xyz**: Training dataset.
- **valid.xyz**: Validation dataset.
- **potential.mtp**: Machine-learned moment tensor potential file with the following atom type mappings:
  - Type 0: Hydrogen (H)
  - Type 1: Oxygen (O)
  - Type 2: Ruthenium (Ru)

## License

This dataset is made available under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/). You are free to share and adapt the material for any purpose, provided you give appropriate credit to the original authors.

## Contact

For any questions or issues regarding this dataset, please contact the corresponding authors of the paper.

---

We hope this dataset will be useful for your research. Thank you for your interest!

