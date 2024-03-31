# Question-Oriented Hierarchical Transport Model

## Introduction
In the quest to advance molecular electronics, our laboratory (http://39.107.98.173/) has developed the Question-Oriented Hierarchical Transport Model, an autonomous method designed to fill the significant void between the simplicity of physical models and the complexity of ab initio quantum transport methods. This tool stands out by offering a novel approach to calculating charge transport in molecular junctions, tailored to address practical research challenges directly.
![model diagram](https://github.com/yuxi-TJU/Question-oriented-Hierarchical-Transport-Model/assets/68102657/82a0ddf0-5b75-4395-83de-b147ab1b33fd)


## Innovative Approach
At its core, this method leverages a hierarchical strategy to simplify device structures, coupled with an optimized calculation precision strategy, ensuring both efficiency and accuracy. It integrates advanced computational techniques, including Extended Hückel Molecular Orbital Theory (EHMO), Semi-Empirical Density Functional Tight Binding (DFTB), and the Non-Equilibrium Green's Function (NEGF) method. To enhance its computational performance, our model utilizes the wide-band approximation and energy level renormalization (DFT+Σ correction), enabling the precise calculation of charge transport properties at an atomic scale.


## Performance and Benefits
The Question-Oriented Hierarchical Transport Model distinguishes itself through its hierarchical approximation strategy and multiple optimization techniques. Benchmark tests against mainstream transport calculation software have demonstrated its ability to achieve significant speed improvements—by orders of magnitude—without sacrificing accuracy. This makes it an invaluable tool for researchers aiming to explore and understand the charge transport properties of molecular junction devices with high efficiency.


## Demonstration
To illustrate the practical application and effectiveness of our hierarchical TB transport model, we present a detailed protocol using the 1,3-BDT molecule, known for its destructive quantum interference (DQI) feature, as a case study.
![workflow](https://github.com/yuxi-TJU/Question-oriented-Hierarchical-Transport-Model/assets/68102657/ad6b807a-0ff2-4671-bfeb-35191da5049a)


## Model Validation through Diverse Research Examples
In our exploration with the Question-Oriented Hierarchical Transport Model, we have undertaken a nuanced approach towards molecular structure systems based on the specific objectives of our research. Our methodology involves varying degrees of simplification of the molecular systems, categorized into three distinct modeling systems for clarity and precision: the bare molecule, the extended molecule, and the device.
![systemsize](https://github.com/yuxi-TJU/Question-oriented-Hierarchical-Transport-Model/assets/68102657/08633bdc-b88c-4fe8-a4ed-246e80276e33)

To demonstrate the versatility and robustness of our model, we selected six representative systems that have been previously reported in experimental research works by scholars in the field. These systems serve as benchmarks, allowing us to validate the accuracy and efficiency of our model, as well as its practical utility in addressing real-world scientific problems. Here is a brief introduction to the origins and characteristics of these six systems:

### System 1:  controlled Quantum Interference in π-Stacked Dimers
- **Reference**: [Nature Chemistry, 2016, 8 (12), 1099–1104.](https://www.nature.com/articles/nchem.2615)
- **Model Treatment**: Bare molecule + EHMO.

### System 2: Fano Resonance in Non-neutral molecule
- **Reference**: [Angewandte Chemie International Edition, 2022, 134 (40), e202210097.](https://onlinelibrary.wiley.com/doi/10.1002/anie.202210097)
- **Model Treatment**: Bare molecule + charge self-consistent EHMO.

### System 3: Quantum Interference in Heterocyclic Molecule
- **Reference**: [Physical Chemistry Chemical Physics (PCCP), 2013, 16 (2), 653–662.](https://pubs.rsc.org/en/content/articlelanding/2014/cp/c3cp53866d)
- **Model Treatment**: Bare molecule + DFTB with higher accuracy.

### System 4: binary conductance in the same junction for contact interface changes
- **Reference**: [Nature Nanotechnology, 2009, 4 (4), 230–234.](https://doi.org/10.1038/nnano.2009.10)
- **Model Treatment**: Extended molecule + DFTB with the same accuracy as the previous case.

### System 5: Junctions with different govern conducting channels
- **Reference**: [Nano Letters, 2012, 12 (1), 354–358.](https://pubs.acs.org/doi/10.1021/nl203634m)
- **Model Treatment**: Device + energy level alignment to the Fermi level of the electrodes + DFTB with the same accuracy as the previous case.

### System 6: Biased Ferrocenyl Rectifier
- **Reference**: [Nature Communications, 2015, 6, 6324.](https://www.nature.com/articles/ncomms7324)
- **Model Treatment**: Device under external electric field + DFTB with the same accuracy as the previous case.
