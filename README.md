# libgrpp
A library for the evaluation of molecular integrals of the generalized relativistic pseudopotential operator (GRPP) over Gaussian functions.

# Features

* basis functions:

  * Cartesian contracted GTOs
  * max angular momentum of basis functions $l_{max} = 10$ (up to $n$-functions, can be increased by hands)

* RPP integrals:
  * scalar-relativistic part: integrals over the local potential (type 1 integrals)
  * scalar-relativistic part: integrals with angular projectors (type 2 integrals)
  * integrals over the effective spin-orbit (SO) interaction operator
  * integrals over GRPP-specific non-local terms (with projectors onto subvalence shells)

* other one-electron integrals:
  * overlap integrals
  * nuclear attraction integrals

* C and Fortran 90 interfaces

* no dependence on external libraries
  * GNU Scientific Library (GSL) comes with LIBGRPP and haven't to be build separately

# Citation
A. V. Oleynichenko, A. Zaitsevskii, N. S. Mosyagin, A. N. Petrov, E. Eliav, A. V. Titov.

LIBGRPP: A Library for the Evaluation of Molecular Integrals of the Generalized Relativistic Pseudopotential Operator over Gaussian Functions.

Submitted to <i>Symmetry</i>, 2022

doi: [10.20944/preprints202212.0530.v1](https://dx.doi.org/10.20944/preprints202212.0530.v1)

```
@article{Oleynichenko2022,
  title = {{LIBGRPP}: A library for the evaluation of molecular integrals of the generalized relativistic pseudopotential operator over {G}aussian functions},
  author = {A. V. Oleynichenko and A. Zaitsevskii and N. S. Mosyagin and A. N. Petrov and E. Eliav and A. V. Titov},
  year = {2022},
  journal = {Submitted to Symmetry},
  doi = {10.20944/preprints202212.0530.v1},
  url = {https://doi.org/10.20944/preprints202212.0530.v1}
}
```

# Bug report
Alexander Oleynichenko, alexvoleynichenko@gmail.com

# References: more on algorithms used

* type 1 integrals (local part):

  * L. E. McMurchie, E. R. Davidson. One- and two-electron integrals over Cartesian Gaussian functions. [<i>J. Comput. Phys.</i> 26, 218 (1978)](https://doi.org/10.1016/0021-9991(78)90092-X)

  * J. O. Jensen, A. H. Carrieri, C. P. Vlahacos, D. Zeroka, H. F. Hameka, C. N. Merrow. Evaluation of one-electron integrals for arbitrary operators $V(r)$ over Cartesian Gaussians: Application to inverse-square distance and Yukawa operators. [<i>J. Comput. Chem.</i> 14, 986 (1993)](https://doi.org/10.1002/jcc.540140814)

  * B. Gao, A. J. Thorvaldsen, K. Ruud. GEN1INT: A unified procedure for the evaluation of one-electron integrals over Gaussian basis functions and their geometric derivatives. [<i>Int. J. Quantum Chem.</i> 111, 858 (2011)](https://doi.org/10.1002/qua.22886)

* type 2 integrals (semilocal part):

  * L. E. McMurchie, E. R. Davidson. Calculation of integrals over ab initio pseudopotentials. [<i>J. Comput. Phys.</i> 44, 289 (1981)](https://doi.org/10.1016/0021-9991(81)90053-X)

  * C. K. Skylaris, L. Gagliardi, N. C. Handy, A. G. Ioannou, S. Spencer, A. Willetts, A. M. Simper. An efficient method for calculating effective core potential integrals which involve projection operators. [<i>Chem. Phys. Lett.</i> 296, 445 (1998)](https://doi.org/10.1016/S0009-2614(98)01077-X)

  * R. Flores-Moreno, R. J. Alvarez-Mendez, A. Vela, A. M. Köster. Half-numerical evaluation of pseudopotential integrals. [<i>J. Comput. Chem.</i> 27, 1009 (2006)](https://doi.org/10.1002/jcc.20410)

  * C. van Wüllen. Numerical instabilities in the computation of pseudopotential matrix elements. [<i>J. Comput. Chem.</i> 27, 135 (2006)](https://doi.org/10.1002/jcc.20325)

  * R. A. Shaw, J. G. Hill. Prescreening and efficiency in the evaluation of integrals over ab initio effective core potentials. [<i>J. Chem. Phys.</i> 147, 074108 (2017)](https://doi.org/10.1063/1.4986887)

* spin-orbit integrals:

  * R. M. Pitzer, N. W. Winter. Spin-orbit (core) and core potential integrals. [<i>Int. J. Quantum Chem.</i> 40, 773 (1991)](https://doi.org/10.1002/qua.560400606)

* integrals non-local terms (with projectors onto subvalence shells):

  * A. V. Oleynichenko, A. Zaitsevskii, N. S. Mosyagin, A. N. Petrov, E. Eliav, A. V. Titov. LIBGRPP: A library for the evaluation of molecular integrals of the generalized relativistic pseudopotential operator over Gaussian functions. [Submitted to <i>Symmetry</i> (2022).](https://dx.doi.org/10.20944/preprints202212.0530.v1)

