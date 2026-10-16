---
layout: page
title: Lecture 2 Notes
category: MIT3320OCW
permalink: /Lec2Notes/
order: 2
---
[Lecture Slides](https://ocw.mit.edu/courses/3-320-atomistic-computer-modeling-of-materials-sma-5107-spring-2005/resources/2_03_note/)

[Lecture Video](https://www.youtube.com/watch?v=kHdqdTe7G44)


## Lecture 2: Potentials, Supercells, Relaxation, Methodology

### System Sizes and Periodicity

Finite System (molecule or cluster)
- No Problem -> simply use all the atoms!

Infinite System (liquids or solids)
- Do not approx. as finite -> use Periodic Boundary Conditions

For defect calculations unit cell becomes a **Supercell**

### How large should the supercell be?

Investigate Convergence! **(check BIG and SMALLER)

Direct interactions from Energy Expression (potential)

Indirect interactions (long range) + (elastic/relaxation)

For charge defects electrostatic interactions are long-ranged and special methods may be necessary

### Effective Medium Theories: The Embedded Atom Method

Problem w/ Potentials
-cohesive energy depends on # of bonds, **But non-linearly**

Solution
- Write energy per atom as $$E = f*(number of bonds)$$ where f is the non-linear function --> **Energy Functionals**

Embedded Atom Method (EAM)
- proximity measured by e- density on central atom

### EAM: Physical Concept (Justification)
Bonding energy (embedding energy) due to ***Electron Delocalization***

### Issues and problems with EAM

Bonding is spherical:
-Limitation in early transistion metals and covalent systems --> **MEAM**

Potential is NOT unique:
-Some part of the energy can be divided arbitrarily between pair potential and embedding

Limitations in Alloys:
-In elements, any error arising from using the atomic electron density is absorbed when the embedding function F is fitted.

### Modified Embedded Atom Method (MEAM)

Embedding functions that keep track f the angular dependencies by converting the problem onto spherical harmonics
