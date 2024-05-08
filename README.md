# Question-Driven Hierarchical Computation (QDHC) Transport Model

## Introduction
The Question-Driven Hierarchical Computation Transport method was developed in our laboratory (http://39.107.98.173/) as an autonomous method designed for the computation charge transport in molecular jucntion and molecular devices. By fullfilling the significant space between the conceptual ideal physical models and the ab initio quantum transport computation with hierarchical computational methods, this tool offers high performance computaion on charge transport in molecular junctions, with significant lower computational cost without losing accuracy compared with the main stream quantum transport computation packs based on DFT+NEGF.
![model diagram](https://github.com/yuxi-TJU/Question-oriented-Hierarchical-Transport-Model/assets/68102657/82a0ddf0-5b75-4395-83de-b147ab1b33fd)
![systemsize](https://github.com/yuxi-TJU/Question-oriented-Hierarchical-Transport-Model/assets/68102657/08633bdc-b88c-4fe8-a4ed-246e80276e33)

## Innovative Approach
Our strategy employs a hierarchical methodology in handling device structures and utilizes appropriate approximations combined with computation techniques of optimized precision to ensure both efficiency and accuracy. It incorporates various level quantum chemistry computational methods, ranging from the simplest Extended Hückel Molecular Orbital Theory (EHMO) to the more complex Semi-Empirical Density Functional Tight Binding (DFTB) for electronic structure calculations, tailored to the problem's specifics. For transport calculations, we employ the Non-Equilibrium Green's Function (NEGF) method with pre-defined precise numerical electrode self-energy, which significantly reduced computational demands by eliminating the need for repetitive electrode calculations. Moreover, our model enhances transport computation precision through energy level renormalization correction (DFT+Σ correction), precisely adjusting the molecule-electrode energy level alignment. This advancement enables accurate determinations of charge transport properties at the atomic level, streamlining the computational process while maintaining high precision.


## Performance and Benefits
The Question-Driven Hierarchical Transport Model stands out with its hierarchical approximation strategy and multiple optimization techniques. Benchmark tests against leading transport calculation software have shown its capability for significant speed improvements—orders of magnitude faster—without compromising accuracy. This efficiency makes it an indispensable tool for the study of charge transport in molecular junction devices and the design of molecule devices.


## Demonstration
To illustrate the practical application and effectiveness of our hierarchical TB transport model, we present a detailed protocol using the 1,3-BDT molecule, known for its destructive quantum interference (DQI) feature, as a case study.
![workflow](https://github.com/yuxi-TJU/Question-oriented-Hierarchical-Transport-Model/assets/68102657/ad6b807a-0ff2-4671-bfeb-35191da5049a)


## Model Validation through benchmark studies
In our exploration with the Question-Driven Hierarchical Transport Model, we have undertaken a nuanced approach towards molecular structure systems based on the specific objectives of our research. Our methodology involves varying degrees of simplification of the molecular systems, categorized into three distinct modeling systems for clarity and precision: the bare molecule, the extended molecule, and the device.

To demonstrate the versatility and robustness of our model, we selected six representative systems that have been previously reported in experimental research works by scholars in the field. These systems serve as benchmarks, allowing us to validate the accuracy and efficiency of our model, as well as its practical utility in addressing real-world scientific problems. Here is a brief introduction to the origins and characteristics of these six systems:

### System 1:  controlled Quantum Interference in π-Stacked Dimers
- **Reference**: [Nature Chemistry, 2016, 8 (12), 1099–1104.](https://www.nature.com/articles/nchem.2615)
- **Model Treatment**: Bare molecule + EHMO.
![case1](https://github.com/yuxi-TJU/Question-driven-Hierarchical-Transport-Model/assets/68102657/06c971bf-71f8-4d0e-aeba-772bd2884e5d)

### System 2: Fano Resonance in Non-neutral molecule
- **Reference**: [Angewandte Chemie International Edition, 2022, 134 (40), e202210097.](https://onlinelibrary.wiley.com/doi/10.1002/anie.202210097)
- **Model Treatment**: Bare molecule + charge self-consistent EHMO.
![case2](https://github.com/yuxi-TJU/Question-driven-Hierarchical-Transport-Model/assets/68102657/2d3e9b53-9f78-499a-831d-7fc74e4ba4ba)

### System 3: Quantum Interference in Heterocyclic Molecule
- **Reference**: [Physical Chemistry Chemical Physics (PCCP), 2013, 16 (2), 653–662.](https://pubs.rsc.org/en/content/articlelanding/2014/cp/c3cp53866d)
- **Model Treatment**: Bare molecule + DFTB with higher accuracy.
![case3](https://github.com/yuxi-TJU/Question-driven-Hierarchical-Transport-Model/assets/68102657/8f20778c-b85c-4514-abdb-afed86db17c1)

### System 4: binary conductance in the same junction for contact interface changes
- **Reference**: [Nature Nanotechnology, 2009, 4 (4), 230–234.](https://doi.org/10.1038/nnano.2009.10)
- **Model Treatment**: Extended molecule + DFTB with the same accuracy as the previous case.
![case4](https://github.com/yuxi-TJU/Question-driven-Hierarchical-Transport-Model/assets/68102657/c2c1eb2f-46c1-4892-9290-415acbf4b7ec)

### System 5: Junctions with different govern conducting channels
- **Reference**: [Nano Letters, 2012, 12 (1), 354–358.](https://pubs.acs.org/doi/10.1021/nl203634m)
- **Model Treatment**: Device + energy level alignment to the Fermi level of the electrodes + DFTB with the same accuracy as the previous case.
![case5](https://github.com/yuxi-TJU/Question-driven-Hierarchical-Transport-Model/assets/68102657/08035492-a13e-4c8d-aeea-3058e56529eb)

### System 6: Biased Ferrocenyl Rectifier
- **Reference**: [Nature Communications, 2015, 6, 6324.](https://www.nature.com/articles/ncomms7324)
- **Model Treatment**: Device under external electric field + DFTB with the same accuracy as the previous case.
![case6](https://github.com/yuxi-TJU/Question-driven-Hierarchical-Transport-Model/assets/68102657/199efa73-40d8-45e9-869c-2d5a6dead373)
