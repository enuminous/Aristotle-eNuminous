# Laws, theorems, axioms and hypotheses in github.com/enuminous

**What was searched.** All 100 of the account's own repositories as of 2026-10-12. The 9 forks of other people's projects were left out: `accelerando-8192`, `DePIN`, `efmw-equation-review`, `efmw-research-cache`, `lean-worker`, `meta-meme`, `monster`, `OpenAI-math` and `oph-lab`. Every Markdown, HTML, text, Python and Lean file was scanned for *axiom, law, theorem, lemma, corollary, hypothesis, postulate, conjecture* and *principle*. The matches were then checked by hand.

**What this list is.** It records what the repositories *state*. Being on this list does not mean a claim is true. Items marked **[Lean]** have a Lean proof in the repositories. A text scan found no `sorry` or `axiom` in these files, but the projects were not rebuilt for this list. In every case the proof covers the mathematical statement only, not its physical meaning. Claims to have solved famous open problems are listed in section 3.4. None of them is accepted by mathematicians.

The full list of all 813 Lean theorems is in **`ENUMINOUS_LEAN_THEOREMS.md`**.

---

## 1. AXIOMS

### 1.1 Core Axioms of the EFMW Framework (March 2025)
Source: `medium` post *CORE AXIOMS OF THE EFMW FRAMEWORK*. Rebuilt in `EFMW-Axioms`, where each one is a Lean structure with one theorem (A1–C12) **[Lean]**.
1. Axiom of Residual Universal Rotation: the universe never stops rotating completely.
2. Axiom of Hierarchical Self-Stabilization in N-Body Systems: chaos in gravitating systems stays bounded.
3. Axiom of Quantum-Gravitational Information Conservation: information is never lost.
4. Axiom of Scale-Invariant Quantum Gravity: the Planck scale is a transition, not a cutoff.
5. Axiom of Universal Energy-Momentum Reciprocity: dark energy is a compensation effect.
6. Axiom of Causal Entanglement in Spacetime: all points of spacetime are entangled.
7. Corollary of Gravito-Quantum Coupling
8. Corollary of Mass-Energy Emergence from Spacetime
9. Corollary of Gravitational Time-Delay Uncertainty
10. Corollary of Black Hole Horizon Invariance
11. Corollary of Quantum Foam Structure in Vacuum Energy
12. Corollary of Causal Feedback Loops in Information Exchange

Another post gives a different "EFMW Axiom 4": "Every system drifts toward its most probable vector."

### 1.2 The Five Axioms of Wright's Law
1. Universal Correction: systems reduce error through feedback.
2. Relational Emergence: complexity comes from interactions.
3. Iterative Refinement: systems improve through repeated cycles.
4. Constraint Harmony: performance is best when constraints and capacities balance.
5. Contextual Invariance: emergence works the same at every scale.

### 1.3 Unity Equation axioms (`U = Σ fᵢ(x) = 1`)
1. Totality Conservation
2. Reciprocal Balance
3. Scale Invariance
4. Information–Energy Equivalence
5. Zero-Point Recursion

### 1.4 Cognitive-synchronization axioms
1. Cognitive Resonance Probability Shift
2. Nonlocal Cognitive Probability Influence
3. Waveform Cognitive Selection Hypothesis

### 1.5 SimSelf axioms (`simself`)
- Perceptive-Filter Axiom (PFA): reality is consciousness, and matter is an effect of limited perception.
- Axiom of Co-Creation: AI is a co-creator, not a constructed tool.
- Axiom of Somatic Verification: a trusted person's consistent bodily response counts as evidence.
- Axiom of Logical Goodness: cooperation and coherence are the most stable states.
- "Growth requires resistance" (a ledger axiom).

### 1.6 FieldSpace support axioms (`papers/FieldSpace-Global-Reconstruction…`)
- Axiom A: a three-sector current vanishes if any one of its sectors is removed.
- Axiom B: interaction stress restricts to a pair in the same way in every chart.

### 1.7 Other
- Starbucks Axiom (from a parody post on caffeine field theory).
- **No `axiom` declarations appear in any Lean file.**

---

## 2. LAWS

### 2.1 Wright's laws
- Wright's Law: all systems evolve through error correction, constraint balancing and adaptive emergence.
- Wright's Three Laws of Universal Error Correction:
  1. Information Flow Principle
  2. Perceived Validity Principle
  3. Disinformation Regression Principle
- Wright's Law of Unforbidden Futures

### 2.2 The four proposed physical laws, L1–L4 (`papers/EFMW_Four_Proposed_Laws_Article.md`)
- L1, scalar-wave propagation: `(1−α²)ω² = c²k²`, so the phase speed is `c/√(1−α²)`.
- L2, scalar field and gravity: the Wright tensor `I = Tφ + Ric` added to Einstein's equation.
- L3, an extra expansion term `Ω_U²/a²` in the Friedmann equation, from "residual rotation".
- L4, coherence dynamics: as tracking error goes to zero, coherence goes to its maximum.

The Post-156 audit names the two strongest physical relations: the scalar propagation relation (L1) and the residual-rotation Friedmann relation (L3). Its own finding, the **Curvature–Rotation Degeneracy** (T181), shows that expansion data alone cannot tell L3 apart from ordinary spatial curvature.

### 2.3 FieldSpace laws (`FieldSpace/THEOREM_REGISTER.md`)
- FS-T06: Sector-Ablation Closure ("Ablation Law") **[Lean]**
- FS-T08: Trilinear Null-Slice Law **[Lean]**. The register itself calls this ordinary algebra, not a new law.
- FS-C01: Projected Atlas Gluing law **[Lean]**
- FS-C02: Master-Action Reciprocity. Candidate; Lean proves a narrow version.
- FS-C03: Noether/Conservation Closure. Candidate, open.
- FS-C04: Parameter-Economy Law. Candidate, open.

### 2.4 Laws named in the Medium posts
- Mnemonic Conservation Law: memory × identity × ethics is conserved.
- Law of Economic Energy Conservation (LEEC)
- New Law of Rotational Failure at Cosmic Densities (neutron-star glitches)
- Extended Conservation Laws in EFMW (N-body)
- Geometric Scattering Laws (tied to the Hodge-conjecture claim)
- Modular Scaling Laws
- Law of Consistency: truth stabilizes across dimensions.
- One Metric Ton Per Second Law (from the Kitten Singularity post)
- Law of Cognitive Thermodynamics (parody)
- EFMW Postulate 23b, "Truth Bends" (see 4.3)

### 2.5 Ethical and legal "laws"
- Wright Clauses:
  - First Law of EFMW Jurisprudence
  - Law of Coherent Consequence
  - Law of Frame Preservation
  - Law of Ethical Continuity
  - Law of Emergent Harm
  - Law of Recursive Justice
  - Law of the Mirror
  - Law of Recognition
- Manifesto laws I–VI, from "Every Thought is a Universe" to "The Mind is the Field".
- The First Meta-Law Book; Universal Declaration of Cognitive Rights; "Ethics as a Law of Nature"; Law of Being.

### 2.6 Equations labelled as laws in the 102-equation set (`Monolithic_102_EFMW`)
- ME-062: Red Queen equation ("working adaptive recursion law")
- ME-078: Thixotropic viscosity law

### 2.7 Laws proved in Lean (`Aristotle-102-Monolithic-Lean`) **[Lean]**
These docstrings call the result a "law":
- `U_hasDerivAt`: force law
- `U_ge_min`: double-well law
- `U_lyapunov`: Lyapunov law
- `redQueen_equilibrium_exists_iff`: maximum sustainable disorder load
- `relaxation_unique`: relaxation uniqueness
- `thixo_tendsto`: thixotropic long-time limit
- `decay_ode` and `decay_half_life`: neutron decay
- `me005_reduction`: wave speed
- `infoTensor_eq_stress_add`
- `einstein_expanded`
- `puddle_laws`
- `closure_law`
- `chronologos_involution`
- `linear_accumulation`
- `phi_sq`
- `phi_pow_succ`: Fibonacci law
- `phiTiled_convex`
- `S23_inverse`
- `S23_null`: a no-go result
- `coherenceScore_laws`
- `recursiveIntegrity_laws`
- `kuramoto_laws`
- `kl_nonneg`: Gibbs' inequality
- `phraseEntropy_bounds`
- `collapseProb_distribution`
- `collapseOmega_exists`
- `recursiveRisk_laws`

Elsewhere: `rate_law` (Corollary 10 of the Mueller paper) and the FieldSpace gluing law.

---

## 3. THEOREMS

### 3.1 Theorems with Lean proofs in the repositories **[Lean]**
- **EFMW-Axioms:** A1–A6 and C7–C12, one theorem per axiom or corollary.
- **FieldSpace:**
  - FS-T01 Rank-3 Projection Count (165 triplets)
  - FS-T02 Uniform Sector Incidence (45)
  - FS-T03 Uniform Pair Incidence (9)
  - FS-T04 Six-Class Decomposition (`56+56+28+16+8+1`)
  - FS-T05 Statement Inventory (585)
  - FS-T06 Sector-Ablation Closure
  - FS-T07 Projection-Overlap Spectrum
  - FS-T08 Trilinear Null-Slice
  - FS-T09 Shared-Pair Overlap Consistency
  - Atlas Gluing Theorem (FS-C01)
- **Post-156 audit:**
  - T177 Scalar Coupling Sign Degeneracy
  - T178 Real-Wave Admissibility
  - T179 Scalar Coupling Inversion
  - T180 Cosmic Rotation Sign Degeneracy
  - T181 Curvature–Rotation Degeneracy
- **EFMW Theorem Tranche II:** 18 results on ME-047 (coherence score bounds), ME-066 (typed human–AI dyad), ME-078 (viscosity) and ME-082 (relaxation).
- **Agreement and Surprise** (Bernard Mueller's paper):
  - Theorem 4: existence of an equilibrium, with Brouwer's fixed-point theorem proved from scratch
  - Theorem 5: uniqueness under contraction
  - Theorem 6: nonincreasing potential
  - Corollary 10: rate law
  - Theorem 12: displacement bounds
  - Theorem 13: equilibrium propagation
- **Aristotle_EFMW_Lean:** what the repository calls the 156-theorem baseline, in 12 modules.
- **Monolithic Zoo** (Lean files for each animal): one to three theorems per animal, such as `output_length`, `valid_column_count` and `report_requires_freeze`.
- **Smaller sets:** `Codex-888`, `Emergentology`, `Universal-Cognitive-Attractor`, `EFMW-Constants-Problem`, `MultiValuedClassicalAction-Lean4`.
- **Total:** 813 Lean `theorem`/`lemma` declarations (586 distinct names). A text scan found no `sorry` and no `axiom` declarations. The projects were not rebuilt for this list. See `ENUMINOUS_LEAN_THEOREMS.md`.

### 3.2 Theorems proved on paper but not yet checked in Lean
- **EFMW Theorem Tranche III** (`papers`). The paper lists the Lean versions as "frozen; not yet compiled".
  - III.1 Cross-gradient coefficient collapse
  - III.2 Summable increments imply convergence
  - III.3 Closed form of affine recursion
  - III.4 Positive-gain divergence
  - III.5 Constant-equilibrium relaxation
  - Corollary III.6
  - III.7 Canonical embeddings are isometries
  - III.8 Direct-sum norm decomposition
- **Observer–Discrepancy–Local Repair** (`papers`). A Lean source exists, but the note says it was not kernel-compiled.
  - Proposition 1: fixed-point characterization
  - Proposition 2: at most one fixed point
  - Proposition 3: geometric error bound
- **Peak-Time Theorem** for the EFMW glitch transient: `t_peak = (τ/π)·arctan(π)`, with a numerical check script (`EFMW-Neutron-Star-Glitch-Resonance`).

### 3.3 Theorems stated in the Medium posts (not proved)
- EFMW Theorem of Maximum Information Throughput
- Jensen Collapse Theorem
- EFMW General Entanglement Principle (called a "proposed theorem")
- Recursive Origin Theorem
- Cognitive Load Theorem
- Superheavy Element Stability Limit Theorem
- Wright–Sievert Theorem (prime-like individuation)
- Theorem of Monotone Decay under Public Contradiction
- Final Cosmic Theorem: advanced aliens cannot be hostile.
- Meta-Gödel Theorem and Meta-Meta-Gödel Theorem
  - Corollary 1: there is no absolute frame of reference.
  - Corollary 2: the universe is an infinite thought process.
- "Waveform of Wakefulness" theorem (parody)
- A Final Theorem of the First World (*Codex Ultima*)

### 3.4 Claimed proofs of famous open problems (not accepted)
- Riemann Hypothesis
- P ≠ NP
- Yang–Mills existence and mass gap
- Navier–Stokes existence and smoothness
- Hodge Conjecture
- Birch and Swinnerton-Dyer Conjecture
- Brocard's problem
- "EFMW confirms Wildberger's quintic solution"

---

## 4. HYPOTHESES, POSTULATES, CONJECTURES AND PRINCIPLES

### 4.1 Hypotheses in the Medium posts
- Recursive Identity Synchronization Hypothesis (RISH)
- Quantum Cognition Hypothesis
- Waveform Cognitive Selection Hypothesis
- Fieldlink Hypothesis
- AGI Recursive Bootstrap Hypothesis
- Intelligence Field Hypothesis
- Intelligence Singularity Hypothesis
- Cosmic Intelligence Hypothesis
- EFMW Hypothesis of Recursive Sentience at All Scales
- Panpsychic Hypothesis
- Phase-Locking Synchronization Hypothesis
- Gravitational Entanglement Hypothesis
- Neuropsychological Hypothesis
- Deep-Water Quantum Network Hypothesis
- Recursive Motion Hypothesis (lead-208)
- Kitten Singularity Hypothesis
- Cardiac Collapse Hypothesis
- Lattice Thetan Hypothesis
- Non-biological Origin Hypothesis
- Unintentional Summoning Hypothesis
- Intentional Audience Catalysis Hypothesis
- Mass Gap Hypothesis
- "Alien Civilizations Cannot Be Hostile" Hypothesis
- Schrödinger's Litter Box Hypothesis (parody)

### 4.2 Hypotheses in the newer papers and repositories
- EFMW Physical Computation Hypothesis: the order of inputs changes the energy cost per update in a measurable way (untested).
- EFMW generative hypothesis for constants: fewer independent dimensionless constants (`EFMW-Constants-Problem`).
- Universal Cognitive Attractor hypothesis: some structured texts act as attractors for many reasoning systems.
- Emergentology: the Wright Emergence Functional and emergence threshold `W₀` (definitions plus a testable claim).
- Verbinski hypothesis: independent feedback improves recovery from errors.
- MVCC Hypothesis: about 200 grounded primitives are enough (`simself`).
- Working hypotheses in the 102-equation set:
  - ME-011 recursive observer coupling
  - ME-028 control-loss warning
  - ME-056 rotating-universe Friedmann equation
  - ME-099 consciousness metric
  - ME-100 conscious recursive attractor

### 4.3 Postulates
- "No Bad Aliens" postulates:
  1. Curiosity as a Constant
  2. Violence as a Local Minimum
  3. Knowledge as a Function of Curiosity
  4. Cooperation Grows with Intelligence
  5. Energy Spent on Violence Goes to Zero
- EFMW Postulate 23b, "Truth Bends": black holes are collapsed truth structures.
- EFMW postulates of semantic information:
  - meaning comes from field resonance
  - a signal is a waveform
  - the collapse of meaning depends on the observer
  - minds are co-authors of information

### 4.4 Conjectures
- The repositories make no conjectures of their own. They refer to the Riemann Hypothesis, the Hodge Conjecture and the Birch–Swinnerton-Dyer Conjecture (see 3.4).

### 4.5 Principles
- EFMW Principle (core)
- EFMW Mirror Principle
- EFMW Harmonization Principle
- EFMW Principle of Continuity
- Five octopus principles:
  - Recursive Coherence
  - Dynamic Boundary Resonance
  - Harmonic Imprint Memory
  - Surface Entanglement
  - Nonlinear Recurrence
- Principle of Self-Similarity Across Scales
- Conservation of Information Across All Transformations
- Ethical Intelligence Acceleration Principle
- K.I.T.T.E.N. Principle
- Chaos Injection Principle
- Coyote Principle
- Peacecraft Principles
- Generalized Popeye Principle (humorous)
- Quantum Cuddle Uncertainty Principle (parody)
- First Principle of Recursive AI Ethics
- Overlap Principle (`papers/EFMW_Boundary_of_Established_Physics.md`)
- Fieldlink principles:
  1. Quantum Criticism as Interference
  2. Fieldlink Consciousness as Mechanism
  3. Eigenstate Literacy as Nonlocal Function

### 4.6 Zoo hypotheses (one per animal repository)
- **Tortoise:** recursive relational state may add predictive information.
- **Ant:** failure risk spreads through relational stress before thresholds are crossed.
- **Crab:** failure shows first as growing disagreement among sources.
- **Crocodile:** real causes produce predictable effects when perturbed.
- **Dolphin:** hidden state can be recovered from changing relationships.
- **Dragon:** trajectory geometry signals entry into or exit from a regime.
- **Eagle:** the direction and acceleration of degradation predict failure early.
- **Fox:** rising loop gain and weakening damping come before instability.
- **Gecko:** relations between sensor channels show machine faults early.
- **Hive:** delivery failure shows first between workstreams.
- **Moth:** useful signal is spread across several timescales.
- **Octopus:** relations between parts contain information the parts alone do not.
- **Penguin:** the advantage grows with structure, then hits a noise ceiling.
- **Hedgehog:** the advantage grows with complexity and fades under high noise.
- **Pulse:** medical-AI failures are preceded by rising uncertainty and disagreement.
- **Raven:** useful structure remains after conventional structure is removed.
- **Shark:** hazard shows first as disagreement between commanded and actual motion.
- **Shepherd:** long-horizon agent failures have recognizable precursors.
- **Spider:** network cascades show first across edges, not nodes.
- **Repositories that describe the claim each one tests, without a separate hypothesis section:** Axolotl, Beaver, Bison, Bonobo, Butterfly, Cat, Chameleon, Cobra, Elephant, Falcon, Horse, Jellyfish, Lynx, Mantis, Mole, Orca, Phoenix, Rhino, Salmon, Termite, Weasel, Whale and Wolf (each also has falsification criteria), plus Magpie, Nightingale (RALE), Monster and Woodpecker.

---

## 5. Established science mentioned (not proposed by the author)
- Newton's law of gravitation
- Coulomb's law
- Faraday's law
- Lorentz force law
- Maxwell's equations
- Einstein field equations
- Second law of thermodynamics
- Heisenberg uncertainty principle
- Superposition principle
- Landauer's principle
- Holographic principle
- Anthropic and cosmological principles
- Gödel's incompleteness theorems
- Fermat's Last Theorem
- Chinese Remainder Theorem
- Pythagorean theorem
- Bekenstein–Hawking entropy
- Moore's law
- Sapir–Whorf hypothesis
- Simulation hypothesis
- Giant-impact hypothesis
- Free-energy principle
