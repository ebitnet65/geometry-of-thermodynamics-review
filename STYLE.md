# Geometry of Thermodynamics Review
## Editorial Style Guide

---

# General Philosophy

The review is intended to be a synthesis rather than a catalog of the literature. Every section should answer two fundamental questions:

1. **What is the underlying physical idea?**
2. **How does it contribute to the development of response geometry?**

The emphasis should remain on interpretation, synthesis, and unification rather than exhaustive derivation. Mathematical developments should illuminate the physics rather than obscure it.

---

# Notation

## Chemical notation

Use the `mhchem` package throughout.

```latex
\usepackage[version=4]{mhchem}
```

Examples:

```latex
\ce{CuGeO3}
\ce{Cu^{2+}}
\ce{3d^9}
\ce{VOPc}
```

---

## Crystal symmetry

Use standard point-group notation in math mode.

```latex
$D_{4h}$
$O_h$
$C_{2v}$
```

---

## Orbital notation

Use conventional crystal-field notation.

```latex
d_{x^2-y^2}
d_{z^2}
t_{2g}
e_g
```

Electronic configurations should use `mhchem`.

```latex
\ce{3d^9}
\ce{3d^{10}}
```

---

## Response quantities

Reserve the following notation throughout the review.

| Symbol | Meaning |
|---------|---------|
| $begin:math:text$C$end:math:text$ | Heat capacity |
| $begin:math:text$\\chi$end:math:text$ | Generalized susceptibility |
| $begin:math:text$\\Omega$end:math:text$ | Mixed response |
| $begin:math:text$G$end:math:text$ | Symmetric response metric |
| $begin:math:text$A$end:math:text$ | Response one-form |
| $begin:math:text$F\=dA$end:math:text$ | Response curvature |

Use subscripts only when the thermodynamic ensemble or independent variables must be specified, e.g.

```latex
C_h
\chi_T
\Omega_{TB}
\Omega_{\beta h}
```

---

# Terminology

Throughout the review distinguish carefully between the following concepts.

## Control manifold

The space of externally controlled thermodynamic variables.

Examples include

- $begin:math:text$\(T\,h\)$end:math:text$
- $begin:math:text$\(T\,B\)$end:math:text$
- $begin:math:text$\(T\,P\)$end:math:text$
- $begin:math:text$\(\\beta\,\\Gamma\)$end:math:text$

---

## Response manifold

The image of the response map.

Examples include

- $begin:math:text$\(C\,\\chi\,\\Omega\)$end:math:text$
- $begin:math:text$\(G\,A\)$end:math:text$
- spectroscopic response coordinates

The distinction between **control manifold** and **response manifold** should be maintained consistently throughout the review.

---

## Types of geometry

Use the following terminology consistently.

### State Geometry

Examples include

- Berry connection
- Berry curvature
- Zak phase
- Quantum metric
- Bures metric
- Fisher information

These characterize the geometry of quantum states.

---

### Thermodynamic Geometry

Examples include

- Weinhold metric
- Ruppeiner metric

These arise from thermodynamic potentials and fluctuation theory.

---

### Response Geometry

This is the principal focus of the review.

Examples include

- covariance matrices
- mixed response
- response metrics
- response one-forms
- response curvature
- response manifolds

Response geometry characterizes **how systems respond**, rather than the geometry of the states themselves.

---

### Observational Geometry

The geometry reconstructed from experimentally accessible observables, particularly spectroscopic response functions.

---

# Microscopic Models

Whenever possible, begin from a microscopic Hamiltonian,

```latex
H =
H_{\rm spin}
+
H_{\rm orb}
+
H_{\rm SO}
+
H_{\rm ph}
+
H_{\rm sp-ph}
+
H_{\rm int}.
```

Then proceed through

```
Hamiltonian
      ↓
Partition Function
      ↓
Free Energy
      ↓
Response Functions
      ↓
Response Geometry
```

For equilibrium systems, emphasize that thermodynamic geometry derives from the **exact differential** of the free-energy functional rather than from direct differentiation of Hamiltonian parameters.

---

# Conceptual Hierarchy

Maintain the following logical development whenever possible.

```
Microscopic Hamiltonian
        ↓
Statistical Ensemble
        ↓
Thermodynamic Potential
        ↓
Response Functions
        ↓
Geometric Structures
```

Different computational frameworks change **how** the response is computed but not **what** the geometric quantities represent.

Examples include

| Framework | Fundamental Object | Response Obtained From |
|-----------|--------------------|------------------------|
| Ising Monte Carlo | Covariance matrix | Fluctuations |
| Spin–Peierls model | Free-energy functional | Thermodynamic derivatives |
| Open quantum systems | Steady-state density matrix | Response derivatives |
| Nonequilibrium systems | Liouvillian | Response one-form and curvature |

---

# Writing Style

- Develop physical ideas before presenting equations.
- Introduce equations only after motivating them.
- Figures should advance the narrative rather than merely illustrate it.
- Captions should be largely self-contained.
- Every major section should conclude with a brief conceptual summary that naturally prepares the transition to the next section.

The review should read as a continuous intellectual development rather than a sequence of independent topics.

---

# Long-Term Vision

The review is intended to establish a unified framework in which diverse geometric constructions arise from different mathematical objects associated with the same underlying microscopic theory.

```
Hamiltonian
      │
      ├────────► Eigenstates ─────────► Berry Geometry
      │
      ├────────► Partition Function ─► Thermodynamic Geometry
      │
      ├────────► Free Energy ─────────► Response Geometry
      │
      └────────► Liouvillian ─────────► Nonequilibrium Response Geometry
```

The central thesis of the review is that **response geometry complements rather than replaces existing geometric frameworks**, providing a unified language for understanding thermodynamic, quantum, and spectroscopic response across equilibrium and nonequilibrium systems.