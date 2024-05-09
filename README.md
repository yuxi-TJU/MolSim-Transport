# **_MolSim-Transport_: A Question-Driven Hierarchical Computation Scheme for Decoding Charge Transport in Molecular Junctions**

## **Introduction**
_**MolSim-Transport**_, a highly efficient computational scheme within the _**Question-Driven Hierarchical Computation (QDHC)**_ framework, has been developed by [Professor Yu Xi's research group](http://39.107.98.173/) at Tianjin University. This scheme integrates several transport models across various levels of approximation, complemented by computational methods of different accuracies. It provides a comprehensive, multi-level solution for analyzing the charge transport properties in molecular junctions.

![hierarchy](https://github.com/yuxi-TJU/Question-driven-Hierarchical-Transport-Model/assets/68102657/e607529f-6e32-45fa-be8f-d2df5df58722)

_**MolSim-Transport**_ bridges the theoretical gap between DFT+NEGF calculations on the full molecular devices and and simplified theoretical models, encompassing a range of simplifications and approximations at various levels. Considering that the charge transport properties of molecular devices are determined by the molecule, electrodes, and their interfacial interactions, transport calculations span multiple physical scales from atoms to devices. Depending on the specific problems studied and the primary factors involved, this approach selectively disregards less impactful secondary factors, focusing instead on those that critically influence system behavior. By effectively applying theoretical methods at different levels of approximation and precision, this strategy achieves greater efficiency while maintaining accuracy, thus enabling more effective exploration of charge transport behaviors in molecular junction systems.

## **Detailed Description of the QDHC Strategy**

The core of the QDHC (Question-Driven Hierarchical Computation) strategy lies in the refined stratification and approximation strategies at two critical levels: defining the computational system scope and selecting computational methods. Considering that a typical molecular device consists of three parts: the molecule, the molecule-electrode interface, and the source/drain electrodes, the QDHC strategy requires researchers to select appropriate computational schemes and levels based on the objectives of their research. MolSim-Transport offers three levels of schemes:

**Level 1 (L1):** The molecule dominates charge transport here, with electrodes and the "molecule-electrode" interface playing secondary roles. The L1 scheme focuses on the intrinsic molecular characteristics using the wide-band approximation and constant self-energy to substitute for electrodes and the "molecule-electrode" interface. This method ranges from the Extended Hückel Molecular Orbital method (EHT) to the Charge Self-Consistent Extended Hückel Theory (CSC-EHT), up to more advanced semi-empirical computational methods, describing molecular electronic properties with varying precision suitable for molecular systems of different characteristics and complexities. Different computational accuracies maintain the simplicity of matrix forms while simplifying the description of electron interactions reasonably.

**Level 2 (L2):** When the focus shifts to the interactions between the molecule and the electrodes, making the "molecule-electrode" interface a significant factor, an extended molecular model including several electrode atoms should be constructed. MolSim-Transport explicitly considers the "molecule-electrode" interface, applying reasonable truncations to the size of electrode clusters. This maintains the accuracy of the coupling matrix description while balancing the system size and computational efficiency. It then uses the constant local density of states (LDOS) approximation of electrodes to generate the self-energy matrix, thus efficiently exploring the charge transport characteristics dominated by interface effects.

**Level 3 (L3):** This level further incorporates the entire electrode structure. MolSim-Transport provides a molecular junction model that includes the complete principal layer of the electrode, using pre-calculated specific electrode surface Green's functions and the coupling matrix of the extended molecule to build the self-energy matrix, thereby avoiding extensive and time-consuming calculations of the electrode. Coupled with strategies such as regional division and the folding of system Green's functions, this greatly enhances computational efficiency. It further considers the effects of electric field polarization, using linear polarization to address molecular junctions under finite bias, thus enabling low-cost studies of molecular junction transport characteristics under limited bias conditions.

## Innovative Approach
Our strategy employs a hierarchical methodology in handling device structures and utilizes appropriate approximations combined with computation techniques of optimized precision to ensure both efficiency and accuracy. It incorporates various level quantum chemistry computational methods, ranging from the simplest Extended Hückel Molecular Orbital Theory (EHMO) to the more complex Semi-Empirical Density Functional Tight Binding (DFTB) for electronic structure calculations, tailored to the problem's specifics. For transport calculations, we employ the Non-Equilibrium Green's Function (NEGF) method with pre-defined precise numerical electrode self-energy, which significantly reduced computational demands by eliminating the need for repetitive electrode calculations. Moreover, our model enhances transport computation precision through energy level renormalization correction (DFT+Σ correction), precisely adjusting the molecule-electrode energy level alignment. This advancement enables accurate determinations of charge transport properties at the atomic level, streamlining the computational process while maintaining high precision.

## **The QDHC Model Framework**
The QDHC model adheres to a structured workflow when applying various levels of precision in simplification, which goes through an entire process from the initial geometric input final calculation of transport properties.
0. Problem Definition
1. Structural Input
2. Hamiltonian Matrix Construction
3. Definition of Electrode Interactions
4. Establishment of Device Green's Function
5. Calculation of Transport Properties

![flowchart](https://github.com/yuxi-TJU/Question-driven-Hierarchical-Transport-Model/assets/68102657/bac5855f-ecce-4467-a208-5a6b774f8ec0)

## **Demonstration**
To illustrate the practical application and effectiveness of our hierarchical TB transport model, we present a detailed protocol using the 1,3-BDT molecule, known for its destructive quantum interference (DQI) feature, as a case study.
![workflow](https://github.com/yuxi-TJU/Question-oriented-Hierarchical-Transport-Model/assets/68102657/ad6b807a-0ff2-4671-bfeb-35191da5049a)


## Model Validation through benchmark studies
To evaluate the performance of MolSim-Transport, it was applied to the following six molecular junction transport cases from the literature, forming a comprehensive benchmark test. These carefully selected cases span all levels of the QDHC strategy, ensuring the breadth and typicality of the test. The rapid replication of these cases demonstrates the high efficiency of the QDHC strategy in handling problems with different precision requirements and its unique ability to capture key factors in the transport process.

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
