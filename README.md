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

### System 1: π-Stacked Dimers with Quantum Interference
- **Reference**: [Nature Chemistry, 2016, 8 (12), 1099–1104.](https://www.nature.com/articles/nchem.2615)
- **Model Treatment**: Bare molecule + EHMO.

### System 2: Fano Resonance Charged Molecule
- **Reference**: [Angewandte Chemie International Edition, 2022, 134 (40), e202210097.](https://onlinelibrary.wiley.com/doi/10.1002/anie.202210097)
- **Model Treatment**: Bare molecule with charge self-consistent Extended Hückel Molecular Orbital (EHMO) theory.

### System 3: Destructive Quantum Interference in Heterocyclic Molecule
- **Reference**: [Physical Chemistry Chemical Physics (PCCP), 2013, 16 (2), 653–662.](https://pubs.rsc.org/en/content/articlelanding/2014/cp/c3cp52837h)
- **Model Treatment**: Bare molecule utilizing Density Functional Tight Binding (DFTB) with higher accuracy.

### System 4
- **Reference**: [Nature Nanotechnology, 2009, 4 (4), 230–234.](https://www.nature.com/articles/nnano.2009.26)
- **Model Treatment**: Extended molecule using Density Functional Tight Binding (DFTB) with higher accuracy.

### System 5
- **Reference**: [Nano Letters, 2012, 12 (1), 354–358.](https://pubs.acs.org/doi/10.1021/nl203634m)
- **Model Treatment**: Device analyzed using Density Functional Tight Binding (DFTB) with higher accuracy.

### System 6: Biased Device Rectifier in Ferrocenyl Molecule
- **Reference**: [Nature Communications, 2015, 6.](https://www.nature.com/articles/ncomms9598)
- **Model Treatment**: Biased device analyzed with Density Functional Tight Binding (DFTB) with higher accuracy.

1. System 1 - π-stacked dimers with mechanically-controlled quantum interference (Nat. Chem. 2016, 8 (12), 1099–1104.); model treatment: bare molecule + EHMO
2. System 2 - This system Fano Resonance charged molecule (Angew. Chem. 2022, 134 (40), e202210097.); model treatment: bare molecule + charge self-consistent EHMO
3. System 3 - This system DQI in the heterocyclic molecule (Phys. Chem. Chem. Phys. 2013, 16 (2), 653–662.); model treatment: bare molecule + DFTB with higher accuracy
4. System 4 - This system (Nat. Nanotech. 2009, 4 (4), 230–234.); model treatment: extended molecule + DFTB with higher accuracy
5. System 5 - This system (Nano Lett. 2012, 12 (1), 354–358.); model treatment: device + DFTB with higher accuracy
6. System 6 - This system biased device rectifier in ferrocenyl molecule (Nat. Commun. 2015, 6.); model treatment: biased device + DFTB with higher accuracy
