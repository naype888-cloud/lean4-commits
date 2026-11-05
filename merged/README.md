# Merged & open — Physlib

Everything contributed to [Physlib](https://github.com/leanprover-community/physlib), the Lean
physics library of the community, by Eduardo Nava Hernández.

[![merged](https://img.shields.io/github/issues-search?query=repo%3Aleanprover-community%2Fphyslib%20is%3Apr%20is%3Amerged%20author%3Anaype888-cloud&label=merged&color=blue)](https://github.com/leanprover-community/physlib/pulls?q=is%3Apr+is%3Amerged+author%3Anaype888-cloud)
[![open](https://img.shields.io/github/issues-search?query=repo%3Aleanprover-community%2Fphyslib%20is%3Apr%20is%3Aopen%20author%3Anaype888-cloud&label=open&color=lightgrey)](https://github.com/leanprover-community/physlib/pulls?q=is%3Apr+is%3Aopen+author%3Anaype888-cloud)

**[▶ Merged pull requests](https://github.com/leanprover-community/physlib/pulls?q=is%3Apr+is%3Amerged+author%3Anaype888-cloud)** ·
[Open pull requests](https://github.com/leanprover-community/physlib/pulls?q=is%3Apr+is%3Aopen+author%3Anaype888-cloud) ·
[Working fork](https://github.com/naype888-cloud/physlib)

## What is in it

- **Robertson and variance of states:** equality case, normalized variance bounds, density states, Robertson determinant, several observables, covariance form.
- **Open tight binding chain:** current operator and eigenstates, maximal current state, Mandelstam–Tamm and Cramér–Rao, speed limit, velocity band, NRS and NRS³ on the cube.
- **Pauli, Dirac, Planck:** maximal anticommuting family, gamma matrices need four dimensions, Planck below Rayleigh–Jeans.
- **Crystals:** Bravais lattices and their embedding by primitive vectors, tetragonal, hexagonal, orthorhombic, rhombohedral, monoclinic, triclinic, several sites per cell.
- **Spectrum and cube:** the energies of the tight binding chain are its whole spectrum; distinct observables of the cube commute iff they lie on different axes.
- **Relativity:** `SL(2, ℂ)` double cover of the restricted Lorentz group, Cayley–Klein rotations.

## Algebras

The algebraic layer all of the above stands on (`PhyslibAlpha/ProbabilisticTheory`, Tom Ole Diem's framework):

| Algebra | What is proved |
|---|---|
| C*-algebra states | Robertson–Schrödinger and its equality case; Robertson 1934 `\|det Ω\| ≤ det Σ` for several observables |
| Hilbert space / density states | variance and Gram defect of vector states; the covariance form, its invariance and Schur's lemma |
| Unital (Schwarz) maps | variances and covariances do not decrease under unital maps |
| Pauli algebra | at most three anticommuting `2 × 2` involutions; the Pauli matrices attain it |
| Clifford algebra | a Clifford family has even size; the gamma matrices need four dimensions |
| Lie algebra `sl(2, ℂ)` | the double cover of the restricted Lorentz group; Cayley–Klein rotations |
| Observables of the cube | one Weyl pair per axis; different axes commute |

## Counts (5 November 2026)

**49 merged**, 5 open: #1972 bond lengths and hypercubic lattices, #1985 triangular and hexagonal lattices,
#1987 nearest neighbours of fcc and bcc as words of axis steps, #1848 and #1849 positive and completely positive
Pauli-diagonal qubit maps (cube and tetrahedron).

Shared work: the algebraic framework and `ProbabilisticTheory` are Tom Ole Diem's; the file
`PhyslibAlpha/ProbabilisticTheory/CStarAlgebra/Uncertainty.lean` carries both names.

Back to [lean4-commits](../README.md).
