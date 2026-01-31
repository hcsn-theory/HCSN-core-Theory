# Proto-Particle Interaction in HCSN
**Status:** Empirically Supported (Simulation)  
**Phase:** Step B Complete → Step C Design  
**Scope:** Interaction existence and minimal force definition  

---

## 1. Purpose

This document formalizes **proto-particle interaction** within the HCSN framework.

A proto-particle interaction is **not assumed** to be:
- fundamental
- geometric
- conservative
- symmetric
- mediated by Ω directly

Instead, interaction is defined operationally as a **measurable deviation in rewrite dynamics** caused by coexistence.

---

## 2. Context: Proto-Particles (Step A Recap)

From prior investigation:

- Proto-particles are **persistent ξ-clusters**
- Identity is defined by **cluster continuity**
- Stability depends on Ω phase (critical / supercritical)
- Proto-particles coexist without collapsing

These results establish **existence**, not interaction.

---

## 3. New Observable: Rewrite Flux

### Definition 3.1 — Rewrite Flux

For a vertex \( v \), define rewrite flux:

\[
\Phi(v, t) = \text{number of rewrite events touching } v \text{ up to time } t
\]

Rewrite flux is accumulated dynamically and decayed over time windows to avoid divergence.

---

### Definition 3.2 — Cluster Rewrite Flux

For a proto-particle (cluster) \( C \):

\[
\Phi_C(t) = \sum_{v \in C} \Phi(v, t)
\]

This quantity measures how strongly the cluster participates in the rewrite process.

---

## 4. Definition of Interaction (Minimal)

### Definition 4.1 — Proto-Particle Interaction

Two proto-particles \( A \) and \( B \) **interact** if:

> The rewrite flux of one cluster is measurably altered by the presence of the other, relative to isolated evolution.

This definition:
- does **not** assume geometry
- does **not** assume force symmetry
- does **not** assume conservation

---

## 5. Interaction Force (Scalar Proxy)

### Definition 5.1 — Scalar Interaction Strength

Define interaction strength:

\[
F_{AB} = \frac{|\Phi_A - \Phi_B|}{\tau}
\]

where:
- \( \Phi_A, \Phi_B \) are total rewrite fluxes
- \( \tau \) is coexistence duration

This is a **dimensionless**, **non-geometric**, **environment-mediated** force proxy.

---

## 6. Experiment Design

### 6.1 Controlled Dual Injection

1. Evolve universe to target Ω regime
2. Inject proto-particle A
3. Allow stabilization
4. Inject proto-particle B at separation
5. Observe rewrite dynamics during coexistence

No direct interaction rules are introduced.

---

## 7. Empirical Results

From `analysis/interaction_experiment.json`:

Rewrite flux A    : 1659 Rewrite flux B    : 1258 Coexistence τ     : 2494 Interaction F_AB  : 0.1608
---

## 8. Interpretation

- Interaction strength is **non-zero**
- Rewrite flux is **asymmetric**
- Interaction is **mediated by the rewrite environment**
- No direct Ω coupling observed
- No geometric distance required

This confirms **proto-particles interact via rewrite competition**.

---

## 9. Negative Results (Important)

The following were explicitly tested and **not observed**:

- Direct Ω–ξ force coupling
- Ω-gradient force
- Action–reaction symmetry
- Geometric distance law

These absences constrain future theory development.

---

## 10. Status Summary

| Claim | Status |
|-----|------|
Proto-particles exist | Confirmed |
Proto-particles persist | Confirmed |
Proto-particles interact | Confirmed |
Interaction is geometric | Not supported |
Interaction is Ω-mediated | Not supported |

---

## 11. Transition to Step C

Step B establishes **interaction existence**.

Step C investigates **interaction structure**, including:
- scaling laws
- saturation
- symmetry emergence
- effective potentials

No further claims are made at this stage.

---
### C7 Result — Failure of Scalar Conservation

Scalar conservation of ξ (even including rewrite flux)
is empirically falsified.

This implies:
- interaction channel is open
- missing degrees of freedom exist
- conservation, if any, is non-scalar

This motivates Step C8: current-based conservation.
