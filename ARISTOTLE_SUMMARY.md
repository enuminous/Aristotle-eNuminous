# Summary of changes for run 4d06a8a9-f164-4289-9e2c-62aff5aa7c6a
I went through all 100 of the account's own repositories at github.com/enuminous and listed every law, theorem, axiom and hypothesis they state. I left out the 9 forks of other people's projects. Being on the list does not mean a claim is true. I did not rebuild any of the Lean projects, so I haven't confirmed that their proofs check.

There are two files:
- **`ENUMINOUS_CATALOG.md`** is the simple list, grouped by type.
- **`ENUMINOUS_LEAN_THEOREMS.md`** lists every Lean theorem: 813 in total, 586 different names, from 20 repositories. Each one shows the first sentence of its description where the file gives one. Some repositories are copies of others, so a few theorems appear twice.

**Axioms**
- The 12 Core EFMW Axioms and Corollaries from March 2025, such as Residual Universal Rotation and Causal Entanglement.
- The Five Axioms of Wright's Law.
- The five Unity Equation axioms and the three cognitive-synchronization axioms.
- The SimSelf axioms, including the Perceptive-Filter Axiom and the Axiom of Co-Creation.
- FieldSpace Axioms A and B.
- No Lean file declares an `axiom`.

**Laws**
- Wright's Law and Wright's Three Laws of Universal Error Correction.
- The four proposed physical laws L1–L4: scalar-wave speed, the Wright tensor in Einstein's equation, an extra rotation term in cosmic expansion, and coherence dynamics.
- An audit in the repositories shows that the rotation term (L3) can't be told apart from ordinary spatial curvature using expansion data alone.
- The FieldSpace laws, FS-T06/T08 and C01–C04.
- Laws named in the Medium posts, such as the Mnemonic Conservation Law and the Law of Economic Energy Conservation.
- The ethical "Wright Clauses" laws.
- About 30 results in the Lean files that are described as "laws".

**Theorems**
- **With Lean proofs:** FieldSpace FS-T01–T09 plus Atlas Gluing, T177–T181, the 18 results in Theorem Tranche II, one theorem per EFMW axiom, and the theorems from Bernard Mueller's paper.
- **Written proofs only:** Tranche III and the Observer–Discrepancy propositions. Their own documents say the Lean versions have not been compiled yet.
- **Stated without proof:** for example the Jensen Collapse Theorem, the Recursive Origin Theorem and the Final Cosmic Theorem.
- **Open problems:** the posts claim proofs of the Riemann Hypothesis, P ≠ NP, Hodge, BSD and others. None of these is accepted by mathematicians.

**Hypotheses, postulates and principles**
- About 25 named hypotheses from the Medium posts, such as RISH, the Fieldlink Hypothesis and the Panpsychic Hypothesis.
- The newer testable hypotheses, such as the Physical Computation Hypothesis and the Universal Cognitive Attractor.
- The "No Bad Aliens" postulates and Postulate 23b.
- The EFMW principles.
- One central hypothesis for each Zoo animal repository. 19 of them have a written hypothesis; the rest only describe what they test.

At the end there is a short list of established science the posts refer to, such as Newton's law and Gödel's theorems.

**How the list was made:** an automatic text search over all files, then checking the matches by hand. It should cover every named item, but an item described without one of the search words (axiom, law, theorem, hypothesis, postulate, conjecture, principle and similar) could be missing. No Lean files were added or changed, so nothing needed building.