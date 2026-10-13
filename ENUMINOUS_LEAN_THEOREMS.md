# All Lean theorems in github.com/enuminous

Every `theorem` / `lemma` declared in a `.lean` file of the owner's own (non-fork) repositories, as of 2026-10-12.
Each line: the name, then the first sentence of its docstring if the file gives one.

Total: **813** declarations (586 distinct names) in 20 repositories. Some repositories are copies of others (marked below), so the same theorem can appear twice.

Text scan only: no `axiom` declarations and no `sorry` were found in any of these files. The projects were not rebuilt here.

## Aristotle-102-Monolithic-Lean (42)

**`RequestProject/Coherence.lean`**

- `U_even` — U is even: coherent states ±Φ are energetically equivalent.
- `U_hasDerivAt` — The force law: U'(Φ) = aΦ³ − bΦ, so the deterministic, uncoupled part of ME-024 (τ Φ̇ = bΦ − aΦ³) is exactly the gradient flow τ Φ̇ = −U'(Φ).
- `U_critical_iff` — Critical points (equilibria of the uncoupled ME-024): for a, b > 0 they are exactly Φ = 0 and Φ = ±√(b/a).
- `U_ge_min` — Double-well law: for a > 0 the potential is bounded below by −b²/(4a), with equality exactly on the coherent states Φ² = b/a.
- `U_lyapunov` — Lyapunov law for ME-024 (uncoupled, noise-free part): along any solution of τ Φ̇ = bΦ − aΦ³ with τ > 0, the coherence potential satisfies d/dt U(Φ(t)) = −(U'(Φ))²/τ ≤ …
- `redQueen_equilibrium` — ME-063 derived from ME-062: dC/dt = 0 iff αC(1 − C/K) = βD − γḊ.
- `redQueen_equilibrium_exists_iff` — New law from ME-063 (maximum sustainable disorder load): for α, K > 0 an equilibrium coherence exists iff the net disorder load satisfies βD − γḊ ≤ αK/4.

**`RequestProject/Dynamics.lean`**

- `relaxation_unique` — Uniqueness law for the relaxation equation ME-082, dη/dt = (η_eq − η)/τ: every solution is η(t) = η_eq + (η(0) − η_eq) e^(−t/τ).
- `relaxation_solves` — Existence half: the exponential relaxation profile solves ME-082.
- `thixo_eq_relaxation` — ME-078 derived from ME-082: the thixotropic law solves the relaxation equation with η_eq = η₀, starts from η(0) = 0, and is the *only* such solution.
- `thixo_tendsto` — ME-078 long-time law: for τ > 0, η(t) → η₀ as t → ∞.
- `decay_ode` — ME-079 law: the density is the unique solution of dρ/dt = −ρ/τₙ with ρ(0) = ρ₀.
- `decay_half_life` — ME-079 half-life law: ρ(τₙ ln 2) = ρ₀ / 2.
- `emergent_time` — ME-075 derived from ME-076: for continuous ω_rec, dΘ/dt = ω_rec(t), i.e. dt = dΘ/ω_rec wherever ω_rec ≠ 0; if ω_rec > 0 everywhere, Θ is strictly increasing, so the em…

**`RequestProject/Fields.lean`**

- `dAlembert_flat` — ME-003 (□φ = g^{μν} ∇_μ∇_νφ) in flat spacetime is ME-004: □φ = (1/c²) ∂²φ/∂t² − ∇²φ, where H is the Hessian of φ at the point.
- `me005_reduction` — ME-005 law: the expanded scalar equation is ((1 − α²)/c²) ∂²φ/∂t² − ∇²φ = (4π/c²)(E + Pc).
- `infoTensor_eq_stress_add` — Law ME-006 = ME-015 + R: the informational tensor is exactly the standard scalar stress-energy tensor plus the Ricci-type term R_{μν}.
- `einstein_expanded` — Law ME-007 ⇔ ME-008: G + Λg = 8πG(T + κI) is the same equation as its expansion G + Λg = 8πG T + 8πGκ[∇φ∇φ − (1/2)g(∇φ)² − gV + R], componentwise.
- `polar_density` — ME-017 from ME-016: for ψ = ρ e^{iθ} with real amplitude ρ, |ψ|² = ρ².
- `puddle_laws` — ME-036/037 law: (i) the two cross-coupling constants enter only through α + β (because the dot product is symmetric), and (ii) the O-equation ME-037 is the S-equation …
- `closure_law` — ME-065 law: in any monoid of transformations, observer–observed closure O_{n+1} = O_n ∘ S_n, S_{n+1} = S_n ∘ O_{n+1} forces S_{n+1} = S_n ∘ O_n ∘ S_n.
- `chronologos_involution` — ME-073/074 law: if time reversal T is an involution and conjugates the forward step U to its inverse (T⁻¹ U T = U⁻¹), then T ∘ U is itself an involution.
- `linear_accumulation` — ME-094 / ME-101 law: with constant coherence C, the linear recursions E_{n+1} = E_n + ΔE·C and I_{t+1} = I_t + λC have closed form E_n = E_0 + n·ΔE·C; in particular th…

**`RequestProject/Golden.lean`**

- `phi_eq_goldenRatio`
- `phi_pos`
- `phi_sq` — Defining law of ME-041: φ² = φ + 1.
- `phi_sub_one` — φ − 1 = 1/φ: the residual weight of ME-046 is the reciprocal of φ.
- `phi_pow_succ` — Fibonacci law: φ^(n+1) = F(n+1)·φ + F(n) for every n.
- `scalar23_closed_form` — ME-042: Φ₂₃ = φ²³ = 28657 φ + 17711 (Fibonacci numbers F₂₃, F₂₂).
- `scalar46_closed_form` — ME-043: Φ₄₆ = φ⁴⁶ = (φ²³)² = 1836311903 φ + 1134903170.
- `veto13_closed_form` — ME-044: V₁₃ = φ¹³ = 233 φ + 144.
- `phiTiled_convex` — ME-046 law: C_φ is the convex combination C_φ[X] = φ⁻¹ • X + φ⁻² • A(φX), with weights φ⁻¹ + φ⁻² = 1.
- `S23_inverse` — ME-085 law: S₂₃ is invertible, with inverse X ↦ φ⁻²³ X.
- `S23_null` — ME-086/088 law (a no-go): since S₂₃ is linear, the "rebirth" of the null state is null, S₂₃(0) = 0, and S₂₃ X = 0 only for X = 0.

**`RequestProject/Metrics.lean`**

- `coherenceScore_laws` — ME-047 law: for ε > 0 the score lies in [0, 1], is symmetric in x, m, and equals 1 exactly when the self-model matches the state (x = m).
- `recursiveIntegrity_laws` — ME-048 law: 0 ≤ I_rec ≤ C ≤ 1; integrity never exceeds state coherence.
- `kuramoto_laws` — ME-091 law: 0 ≤ K ≤ 1, and K = 1 for perfect phase locking.
- `kl_nonneg` — ME-092 law (Gibbs' inequality): for probability vectors p, q with q > 0, D_KL(P‖Q) = Σ p log(p/q) ≥ 0.
- `phraseEntropy_bounds` — ME-034 law: 0 ≤ H ≤ log n for any probability vector on n phrases (the upper bound follows from Gibbs' inequality against the uniform distribution).
- `collapseProb_distribution` — ME-061 law (Born compatibility): whenever some amplitude is non-zero, the collapse probabilities are non-negative and sum to 1.
- `collapseOmega_exists` — ME-059 law: on any finite, non-empty set of candidate outcomes s, the Collapse-Ω selection argmin_s [−ln P(s|ψ) + λ D(s, Φ) − γ R(s)] is well defined (a minimiser exis…
- `recursiveRisk_laws` — ME-089 law: with P(H), C ∈ [0, 1], risk lies in [0, P(H)], and is monotonically non-increasing in coherence C.

## Aristotle-165-Einsteinian-Tensors (33)
*Note: overlaps with `FieldSpace`.*

**`Ablations.lean`**

- `remove_one_remaining`
- `remove_two_remaining`
- `remove_three_remaining`
- `remove_one_deleted`
- `remove_two_deleted`
- `remove_three_deleted`

**`Coupling.lean`**

- `restrict_third_zero` — Removing the third field kills both terms that require that field.
- `restrict_second_zero` — Removing the second field gives the symmetric reduction.
- `trilinear_null_slice_left` — A genuinely mixed trilinear contribution is invisible on either null slice.
- `trilinear_null_slice_right`
- `shared_pair_overlap_consistency` — Two triplet charts that share the same base term and i-j pair coefficient glue exactly on the slice where their respective third fields vanish.
- `triple_ablation_difference` — Triple-term ablation is exact subtraction of that term.

**`Structure.lean`**

- `triplet_count` — Complete rank-3 atlas size.
- `fixed_sector_incidence` — Number of triplets containing a fixed sector.
- `fixed_pair_incidence` — Number of triplets containing a fixed unordered sector pair.
- `scalar_triples`
- `one_gauge_two_scalars`
- `gravity_two_scalars`
- `gravity_gauge_scalar`
- `two_gauges_scalar`
- `gravity_two_gauges`
- `class_partition` — The six structural classes exhaust the complete atlas.
- `statement_inventory` — Expected displayed-statement inventory for a fully populated atlas.
- `overlap_spectrum` — Pair-of-triplet overlap counts sum to all unordered pairs of distinct triplets.

**`Verified.lean`**

- `triplets_card` — FS-T01: there are 165 triplets.
- `sector_incidence` — FS-T02: every sector lies in exactly 45 triplets.
- `pair_incidence` — FS-T03: every pair of distinct sectors lies in exactly 9 triplets.
- `class_counts` — FS-T04: the six-class decomposition 56 + 56 + 28 + 16 + 8 + 1 = 165.
- `classes_exhaustive` — The six classes exhaust the atlas.
- `statement_inventory` — FS-T05: the inventory 45 + 90 + 90 + 360 = 585.
- `ablation` — FS-T06: deleting a set D of k sectors leaves C(11-k,3) triplets, all of which are exactly the triplets of the remaining sectors (closure under vertex deletion).
- `overlap_spectrum` — FS-T07: overlap spectrum of unordered pairs of distinct triplets (sharing 2 / 1 / 0 sectors): 1980 + 6930 + 4620 = 13530.
- `bilinear_reciprocity`

## Aristotle-Agreement-and-Surprise-Global-Equalibrium-from-Local-Repair (97)

**`RequestProject/Averages.lean`**

- `relaxation_integral_identity` — The integrated relaxation equation: x(T) - x(0) = T (R̄_T - x̄_T).
- `agreement_on_average` — **Proposition 8 (Agreement on average).** Along a relaxation trajectory ẋ = R(x) - x in a bounded set X, ‖x̄_T - R̄_T‖ ≤ diam X / T.
- `damped_average_identity` — **Damped discrete identity.** (1/N) ∑_{k<N} (R(x_k) - x_k) = (x_N - x_0)/(η N).
- `damped_average_bound` — **Damped discrete bound.** If the damped sequence stays in a bounded set X, then ‖(1/N) ∑_{k<N} (R(x_k) - x_k)‖ ≤ diam X / (η N).
- `timeAvg_mem` — The time average of a trajectory staying in a closed convex set stays in it.
- `linear_repair_limit_points` — **Corollary 9 (Linear repair).** If X is bounded, closed and convex and R is affine, R x = A x + c, then every limit point of the time averages x̄_T (as T → ∞) of a re…
- `lipschitz_closure_gap` — **Lipschitz closure gap.** For a repair map that is L-Lipschitz on a bounded closed convex X, along a relaxation trajectory in X, ‖R(x̄_T) - x̄_T‖ ≤ diam X / T + (L / …
- `rate_law` — **Corollary 10 (Rate law).** Let each node integrate a weighted sum of signals emitted by its neighbours, Rᵢ(x) = ∑ⱼ Wᵢⱼ sⱼ(xⱼ) + eᵢ, with continuous signals sⱼ, and l…
- `charge_balance` — **Proposition 11 (Charge balance).** Integrated (distributional) form of the spiking equations of node i on the window [0, T]: * current: τ ġᵢ = -gᵢ + τ ∑ⱼ wᵢⱼ ∑ₖ δ(t …

**`RequestProject/Contraction.lean`**

- `contraction_existsUnique_fixedPoint` — **Theorem 5 (1): existence and uniqueness** (Banach).
- `dampedStep_dist` — One damped step contracts with factor 1 - η + η q towards a fixed point.
- `damped_dist_le` — **Theorem 5 (2): damped repair converges geometrically.** With η = 1 this is synchronous repair (damped_one).
- `damped_tendsto` — **Theorem 5 (2), convergence.** Damped (in particular synchronous) repair converges to the fixed point from every start in X.
- `relaxation_dist_le` — **Theorem 5 (3): relaxation converges exponentially.** If x solves ẋ = R(x) - x on [0, ∞) and stays in X, then ‖x(t) - x⋆‖ ≤ exp(-(1-q) t) ‖x(0) - x⋆‖.
- `fixedPoint_lipschitz_evidence` — **Theorem 5 (4): sensitivity to evidence.** If x⋆(e) and x⋆(e') are equilibria under e and e', R(·, e) contracts with factor q < 1, and R is L-Lipschitz in the evidenc…
- `displacement_bounds` — **Theorem 12 (Equilibrium displacement is bounded by disagreement on both sides).** If x⋆ is a fixed point of R which contracts with factor 0 ≤ q < 1, then for any sta…
- `detuning_zero_iff` — **Detuning bound (Section 2).** If the map under the new evidence contracts with factor q and has rest x⋆, its distance from the reference rest x₀ lies between Δ/(1+q)…
- `existsUnique_equilibrium_of_contraction` — **Theorem 5 (1) for repair networks.** If every node's state space is closed and nonempty and R(·, e) contracts on X, the network has exactly one equilibrium under e.
- `equilibrium_displacement` — **Theorem 12 for repair networks.** With x the old agreement and e' the new evidence, the new equilibrium lies at distance between D/(1+q) and D/(1-q) from x, where D …

**`RequestProject/Defs.lean`**

- `globalR_local` — Locality: the repair target of node i depends only on the neighbours of i.
- `globalR_mapsTo`
- `isEquilibrium_iff_nodeDisagreement`
- `isEquilibrium_iff_disagreement`
- `damped_one`
- `dampedStep_fixed_iff` — The rest points of damped repair (η ≠ 0) are exactly the equilibria.
- `dampedStep_mem` — Damped repair stays in a convex domain that R maps into itself.
- `damped_mem`

**`RequestProject/EqProp.lean`**

- `fderiv_partial_fst` — Partial derivative in θ through the full derivative.
- `fderiv_partial_snd` — Partial derivative of F in x through the full derivatives.
- `two_equilibria_give_gradient` — **Theorem 13 (Two equilibria give the gradient; Scellier and Bengio).** Let E be twice continuously differentiable and C differentiable, and let xb be differentiable n…
- `free_state_stationary_nudged` — **No surprise, no learning.** If the free state x₀ is stationary for the energy and the cost is also stationary there (∇ₓ C(x₀) = 0), then x₀ is a stationary point of …
- `no_surprise_no_learning` — **No surprise, no learning (contrast).** If moreover the stationary branch is locally unique — every stationary point of F(θ, β, ·) in a set U ∋ x₀ equals xb β — then …
- `pairwise_energy_partial` — **Pairwise energy.** For a pairwise energy E(θ, s) = -∑_{(i,j) ∈ P} θᵢⱼ sᵢ sⱼ + E₀(s) with one parameter per pair, ∂E/∂θᵢⱼ = -sᵢ sⱼ; hence the two-state contrast for t…
- `two_speed_dissipation` — **Two speeds, one mechanism.** If states and slow variables follow ẋ = -Mₓ ∇ₓF, θ̇ = -ε M_θ ∇_θF with positive semidefinite mobilities and ε ≥ 0, then Ḟ = -⟪∇ₓF, Mₓ ∇ₓ…

**`RequestProject/Existence.lean`**

- `exists_equilibrium` — **Theorem 4 (Existence).** If every node's state space is nonempty, compact and convex, and the global repair map R(·, e) is continuous on X, the network has an equili…

**`RequestProject/Layers.lean`**

- `no_infinite_descent` — **Finite descent.** If every accepted repair strictly lowers a potential that takes only finitely many values, there is no infinite repair sequence.
- `newman` — **Newman's lemma.** A terminating, locally confluent relation is confluent.
- `exists_normal` — Every state of a terminating repair relation reaches some normal form.
- `existsUnique_normal` — **Unique normal form.** A terminating, locally confluent repair relation gives each initial state exactly one reachable normal form; hence every observable of the endp…
- `cycle_sum_eq_zero` — **Cycle obstruction (necessity).** If an assignment x satisfies abelian edge demands x (v (k+1)) - x (v k) = b k around a closed cycle v 0, …, v m = v 0, the signed cy…
- `triangle_no_assignment` — **The triangle over ℤ/2 with demands 0, 0, 1** has no global assignment.
- `triangle_each_edge_satisfiable` — Each edge of the triangle can be satisfied on its own.
- `triangle_mismatch_pos` — The minimum of the mismatch on the triangle is positive: every minimiser contains irreducible residual inconsistency.
- `noise_bound_explicit` — **Noise bound.** If a (m+1) ≤ λ a m + ε with 0 ≤ λ < 1, then a m ≤ λ^m a 0 + ε / (1 - λ).
- `noise_bound` — **Noise bound (limsup a ≤ ε / (1 - λ)).** If a (m+1) ≤ λ a m + ε with 0 ≤ λ < 1 and ε ≥ 0, then for every δ > 0, eventually a m ≤ ε / (1 - λ) + δ.
- `replicator_eq_mobility` — **The shared equation.** The replicator field is M(x) ∇F with ∇F = A x.
- `potential_directional_deriv` — For symmetric A, ∇F = A x, where F(x) = ½ xᵀ A x.
- `mobility_mulVec` — M(x) v = (xᵢ vᵢ - xᵢ (x · v))ᵢ.
- `mobility_one` — M(x) 1 = 0 on the simplex: the mobility preserves total frequency.
- `quadratic_mobility` — **Weighted-variance identity.** On the simplex, vᵀ M(x) v = ∑ᵢ xᵢ (vᵢ - x·v)².
- `mobility_psd` — M(x) is positive semidefinite on the simplex.
- `potential_rate` — **Mean fitness climbs.** Along the replicator dynamics with symmetric payoffs, the rate of change of F = ½ xᵀ A x is ∇Fᵀ ẋ = ∑ᵢ xᵢ (fᵢ - f̄)² ≥ 0.
- `rest_of_equal_fitness` — A state of the simplex at which all present types earn the same is a rest point; in particular if all (A p)ᵢ are equal, p is a rest point of the replicator dynamics.
- `log_balance` — **A population that cycles agrees on average.** If every type stays positive along the replicator dynamics on [0, T], then (log xᵢ(T) - log xᵢ(0)) / T = (A x̄_T)ᵢ - (1…
- `time_average_limit_rest` — **Every limit point of the time averages is a rest point.** Along the replicator dynamics on the simplex, if every type stays bounded away from zero (m ≤ xᵢ(t)), then …

**`RequestProject/Potential.lean`**

- `update_mem`
- `minimiser_le`
- `cyclic_mem`
- `cyclic_antitone` — **Theorem 6, monotonicity.** Φ never increases along cyclic repair.
- `tendsto_Φ` — Φ along a convergent sequence in X.
- `limit_of_targets` — A limit of repair targets along a convergent sequence is the repair target of the limit.
- `tendsto_target` — Repair targets depend continuously on the state (uniqueness of the minimiser and compactness).
- `limit_point_is_equilibrium` — **Theorem 6 (Equilibrium limit points under a potential).** Under unique coordinate minimisers of a continuous potential on a product of compact sets, every limit poin…

**`RequestProject/TwoNodeLoop.lean`**

- `clip_mem`
- `clip_of_abs_le`
- `clip_sq_le`
- `clip_eq_zero`
- `continuous_clip`
- `continuous_R`
- `hypotheses_existence` — The network satisfies the hypotheses of the existence theorem (Theorem 4): the square is nonempty, compact and convex, and R is continuous and maps it into itself.
- `clip_cases`
- `fixed_iff` — **Proposition 7 (uniqueness of the equilibrium).** The only fixed point of R (in the square, or indeed in the whole plane) is (0, 0).
- `R_eq_zero` — R vanishes only at the origin.
- `sq_pos_of_ne`
- `R_linear` — In the disc sq p < 1/16 no clipping happens.
- `sq_tendsto_zero`
- `synchronous_not_tendsto` — **Proposition 7 (synchronous repair).** From any start other than (0, 0), synchronous repair x_{t+1} = R(x_t) does not converge.
- `limit_is_rest` — If a trajectory of ẋ = F(x) with continuous F converges, its limit is a zero of F.
- `relaxation_not_tendsto` — **Proposition 7 (relaxation).** No relaxation trajectory ẋ = R(x) - x that starts away from (0, 0) converges.
- `scalar_relaxation_stays` — A scalar relaxation ẏ = a(t) - y with targets a(t) ∈ [-1, 1] stays in [-1, 1].
- `relaxation_stays_in_square` — **Proposition 7 (invariance).** Relaxation trajectories starting in the square stay in the square, since |Rᵢ| ≤ 1.

**`RequestProject/Brouwer/Ball.lean`**

- `for`
- `exists_retraction` — **Retraction from a fixed-point-free C¹ self-map of the ball.**
- `exists_smooth_approx` — Smooth approximation on the closed ball of a continuous function.
- `brouwer_closedBall` — **Brouwer's fixed-point theorem for the closed unit ball of ℝⁿ.**

**`RequestProject/Brouwer/Convex.lean`**

- `for`
- `exists_proj` — The nearest-point projection onto a nonempty complete convex set: existence and the variational characterisation.
- `exists_retraction_convex` — The nearest-point projection onto K is a continuous retraction onto K.
- `brouwer_euclidean` — Brouwer's theorem for nonempty compact convex subsets of ℝⁿ.
- `brouwer_fixed_point` — **Brouwer's fixed-point theorem.** Every continuous self-map of a nonempty compact convex subset of a finite-dimensional real normed space has a fixed point.

**`RequestProject/Brouwer/DetPoly.lean`**

- `exists_poly_det` — det (id + t • A) is the value at t of a polynomial of degree at most dim E.
- `det_add_smul_eq_sum` — **Lagrange form.** For every t, det (id + t • A) = ∑_{j ∈ nodes} det (id + j • A) · ℓⱼ(t).

**`RequestProject/Brouwer/NoRetraction.lean`**

- `det_ne_zero_of_lower_bound` — A linear map that does not shrink vectors too much has nonzero determinant.
- `range_eq_top_of_det_ne_zero` — A linear map with nonzero determinant is surjective.
- `lower_bound_id_add` — id + A with ‖A‖ ≤ 1/2 has a lower bound ‖v‖/2.
- `det_eq_zero_of_range_orth` — If the derivative of r lies in the orthogonal complement of r x ≠ 0, det = 0.
- `no_C1_retraction` — **No C¹ retraction.**

## Aristotle_EFMW_Lean (157)

**`RequestProject/EFMW/ActionsAndFluids.lean`**

- `action_decomposition` — **ME-009** — the unified EFMW action S = ∫ [(R − 2Λ)/(16πG) + L_matter + L_EM + L_φ + L_rec] decomposes into the sum of its sector actions.
- `semiclassicalEq_no_efmw_sources` — Dropping the EFMW sources recovers the semiclassical Einstein equation.
- `relNavierStokes_inviscid` — With vanishing viscous stress and no external force the model reduces to the relativistic Euler equation.
- `density_stationary_of_uniform_flux` — A spatially uniform mass flux forces the density to be stationary in time.
- `fluidStress_symm` — The fluid stress tensor is symmetric whenever the metric and the shear tensor are.
- `torus888_mem_torus` — The toroidal mapping is well defined: both components land on the unit circle.

**`RequestProject/EFMW/CognitiveFields.lean`**

- `recursiveLagrangian_le` — The divergence penalties can only reduce the recursive Lagrangian.
- `recursiveLagrangian_eq` — Equality holds exactly in the perfectly self-modeling case.
- `recursiveStateEq_lam_zero` — Switching off the recursive coupling recovers the baseline dynamics.
- `orderParamRHS_eq_neg_grad` — **The ME-024 order-parameter equation is gradient descent on the ME-025 coherence potential** in the noiseless, perfectly self-modeling limit with no recursive-closure…
- `gradientFlow_potential_nonincreasing` — **ME-069** — along the noiseless cognitive attractor flow ż = −∇V(z) the potential is nonincreasing: its rate of change is −(V'(z))² ≤ 0.
- `puddleRHS_symm` — With equal cross-coupling constants the system is symmetric under exchanging the system field with the observer field.
- `cognitivePressure_nonneg`
- `cognitivePressure_mono`
- `cognitiveTensor_symm` — The cognitive tensor is symmetric whenever the metric is.
- `cognitiveCurvature_zero_irec` — Without recursive information the cognitive curvature equation reduces to pure thought-density sourcing.
- `phiTiled_eq` — The φ-tiled operator is the affine combination (2 − φ)·A(φX) + (φ − 1)·X, whose weights sum to one.
- `phiTiled_weights_sum`
- `memoryUpdate_gt_iff` — A memory weight grows exactly when contextual coherence outweighs the penalized prediction error.
- `nullPair_consistent` — **ME-087** — the null-pair relation eᵢeⱼ = 0 for nonzero basis elements is consistent: a commutative ring containing two nonzero mutually annihilating elements exists.
- `identityAttractor_iff` — **ME-031** — joint convergence of the state, the self-model and the order parameter to an identity attractor is exactly componentwise convergence.

**`RequestProject/EFMW/Coherence.lean`**

- `coherence_denom_pos`
- `coherenceScore_le_one` — The coherence score never exceeds 1.
- `coherenceScore_pos` — The coherence score is strictly positive: the triangle inequality gives ‖x − m‖ ≤ ‖x‖ + ‖m‖ < ‖x‖ + ‖m‖ + ε.
- `coherenceScore_nonneg`
- `coherenceScore_eq_one_iff` — The coherence score equals 1 exactly when the self-model reproduces the state.
- `abs_recursiveClosure_le_one` — Cauchy–Schwarz bounds the recursive closure functional in [-1, 1].
- `recursiveIntegrity_pos`
- `recursiveIntegrity_le_one`
- `recursiveIntegrity_eq_one_iff`
- `divergence_mono_state` — With nonnegative weights, divergence is monotone in the state error.
- `divergence_nonneg` — With nonnegative weights and nonpositive recursive closure term, divergence is nonnegative.
- `warningCriterion_mono` — The warning criterion is monotone: more divergence, or less coherence, can only trigger a warning that was already triggered.
- `warningCriterion_nontrivial` — The warning criterion is not vacuous: it can both fire and fail to fire.
- `entropicHarmonyGradient_mul`
- `risk_mem_unitInterval`
- `risk_antitone_coherence` — Risk decreases as coherence increases.
- `ethicalWeight_nonneg`
- `gammaMetric_mono` — Γ is monotone in each nonnegative factor, so the ME-100 threshold condition is upward closed in each of Φ, R, C.
- `identityStep_iterate` — Iterating the identity-persistence update n times adds n·λC.
- `identityStep_tendsto_atTop` — With nonnegative coherence gain, identity persistence is nondecreasing and diverges.

**`RequestProject/EFMW/Cosmology.lean`**

- `emergenceForce_restoring_inner` — **The emergence force is restoring.** Inside the coherent well (0 < Φ, Φ² < b/a) the force generated by the ME-025 potential pushes the order parameter up towards the …
- `emergenceForce_restoring_outer` — Outside the well the force points back inwards.
- `fifthForce_const` — A uniform coherence field exerts no fifth force.
- `modifiedGeodesic_beta_zero` — With vanishing scalar coupling the modified geodesic equation is exactly the standard geodesic equation: the extension is conservative in β_φ.
- `friedmann_deviation` — **ME-058** — the cosmic deviation parameter is exactly the rotational contribution.
- `friedmannEFMW_ge` — Residual rotation can only increase the expansion rate.
- `friedmannEFMW_lt_iff` — The increase is strict exactly when the residual rotation is nonzero.
- `effectiveDensity_ge`

**`RequestProject/EFMW/Dynamics.lean`**

- `hasDerivAt_coherencePotential`
- `coherencePotential_critical_iff` — The critical points of the double-well coherence potential are exactly Φ = 0 and Φ² = b/a.
- `coherencePotential_ge` — For a double well (a, b > 0) the potential is bounded below by −b²/(4a), with equality exactly at the two coherent minima Φ² = b/a.
- `coherencePotential_eq_min_iff`
- `cognitivePotential_ge` — The cognitive potential is bounded below on every ball, and grows without bound: it is coercive for a > 0.
- `selfModel_zero`
- `selfModel_hasDerivAt` — The proposed solution really does solve the self-model equation.
- `selfModel_tendsto` — For α > 0 the self-model converges to the tracked state.
- `redQueen_equilibrium_iff` — **ME-063** — the equilibrium condition really is equivalent to vanishing coherence rate.
- `redQueen_equilibrium_exists` — Existence of an equilibrium coherence level: if the environmental demand S = βD − γḊ is nonnegative and does not exceed the maximal adaptive capacity αK/4, then some c…
- `viscosity_hasDerivAt` — **ME-082** — the thixotropic law solves the relaxation equation dη/dt = (η_eq − η)/τ with η_eq = η₀.
- `viscosity_zero`
- `decayDensity_hasDerivAt`
- `emergentPhase_hasDerivAt` — **ME-075** — dt = dΘ/ω_rec: the accumulated phase differentiates back to the recursive frequency, so the corpus relation between dΘ and dt is the fundamental theorem o…
- `emergentPhase_strictMono` — With a nonvanishing recursive frequency the emergent time coordinate is strictly monotone, hence a genuine reparametrization.
- `successive_increments_tendsto_zero` — **ME-096** — a convergent recursion has vanishing successive increments.
- `perturbation_recovery` — **ME-032** — perturbation recovery: if the perturbed trajectory converges to the attractor, the deviation vanishes.
- `lyapunov_negative_tendsto_zero` — **ME-033** — a negative Lyapunov exponent forces the perturbation to decay: if ‖δX(t)‖ ≤ M e^{λt} with λ < 0, then δX(t) → 0.

**`RequestProject/EFMW/GoldenScaling.lean`**

- `phi_eq`
- `phi_sq` — The defining identity φ² = φ + 1.
- `one_lt_phi`
- `phi_pos`
- `scalar46_eq_scalar23_sq` — **ME-043** — the asserted identity φ⁴⁶ = (φ²³)².
- `phi_pow_succ` — Every power of φ is an integer combination of φ and 1 with Fibonacci coefficients: φ^(n+1) = F(n+1)·φ + F(n).
- `scalar23_eq` — Closed form for the Scalar-23 coefficient.
- `scalar23_pos`
- `S23_add`
- `S23_smul`
- `S23_injective`
- `S23_zero` — **ME-086 / ME-088** — the null state is fixed by the Scalar-23 operator, so the recursive rebirth operator R_b = S₂₃ ∘ N produces coherence only from a nonzero seed.
- `phase_sync_unique` — **ME-045** — phase synchronization T = ΔΦ / f: the synchronization interval is the unique time with f · T = ΔΦ.

**`RequestProject/EFMW/Information.lean`**

- `shannonEntropy_nonneg`
- `kl_term_ge` — Pointwise form of the Gibbs inequality.
- `klDivergence_nonneg` — **Gibbs' inequality**: the KL divergence between two probability vectors is nonnegative.
- `shannonEntropy_le_log_card` — The entropy of a probability vector on a nonempty finite alphabet is at most log n.
- `mutualInformation_comm` — Mutual information is symmetric in its two arguments.
- `collapseProb_nonneg`
- `collapseProb_sum_eq_one` — **ME-061 / ME-071** — the collapse probabilities are normalized.
- `collapse_argmin_exists` — **ME-059** — the Collapse-Ω functional is well posed on a finite nonempty outcome set: an argmin exists.
- `kuramoto_nonneg`
- `kuramoto_le_one` — Phase coherence never exceeds one.
- `kuramoto_of_const` — Perfect synchronization gives order parameter one.

**`RequestProject/EFMW/PhysicalTest.lean`**

- `Measurement.Compatible_of_strict`
- `eventually_strictlyCompatible` — Strict compatibility with a finite body of data is an open condition: it holds throughout a neighbourhood of any parameter value satisfying it.
- `no_exact_parameter_verification` — **No physical proof of an exact parameter value.** If a finite body of finite-precision data is strictly compatible with the parameter value θ₀, and the predicted obse…
- `measurement_discriminates` — **A measurement can refute.** If the predictions at two parameter values differ by more than twice the error bar, no reading can be compatible with both: the experimen…
- `falsification_by_measurement` — Concretely, finite data can be flatly inconsistent with a parameter value: the criterion of compatibility is not vacuous.
- `phaseSpeed_zero`
- `sqrt_one_sub_sq_pos`
- `sqrt_one_sub_sq_le_one`
- `le_phaseSpeed` — EFMW scalar waves are never slower than light.
- `lt_phaseSpeed` — A nonzero coupling makes them strictly faster: the prediction is sharp.
- `alpha_sq_le_of_speed_measurement` — **A null result bounds the coupling.** If a measurement of the scalar-wave speed agrees with c to within p, then α²(c+p)² ≤ p² + 2pc.
- `alpha_eq_zero_of_exact_lightspeed` — In the limit of a perfect measurement the bound forces α = 0: an exactly light-speed scalar wave is inconsistent with a nonzero EFMW coupling.
- `phaseSpeed_gap` — The predicted speed is monotone in |α|, so a coupling bounded away from zero puts a definite gap between the EFMW prediction and c.
- `speed_experiment_discriminates` — **A single measurement of sufficient precision decides between α = 0 and |α| ≥ ε.** With error bar smaller than half the predicted gap, no reading is compatible with b…
- `decisive_precision_exists` — Hence a decisive experiment exists in principle: for every coupling bounded away from zero there is a positive precision at which the measurement rules out one of the …
- `OmegaU_sq_le_of_hubble_measurement` — **A null cosmological result bounds the residual rotation.** If the measured expansion rate agrees with the ΛCDM prediction to within δ, then Ω_U² ≤ δ a²; see EFMW.fri…
- `OmegaU_eq_zero_of_exact_hubble` — As the cosmological measurement becomes exact, the bound forces the rotation to vanish.
- `physical_test_asymmetry` — **The epistemic asymmetry, in one statement.** For the EFMW scalar sector: a finite-precision experiment can *refute* a parameter hypothesis (there is a precision at w…

**`RequestProject/EFMW/QuantumSector.lean`**

- `phaseCurrent_const_of_continuity` — **ME-019** — the stationary continuity equation ∇·J = 0 forces the phase current to be spatially constant.
- `gaussianAmplitude_pos`
- `hasDerivAt_gaussianAmplitude`
- `deriv_gaussianAmplitude`
- `d2_gaussianAmplitude` — The Gaussian amplitude satisfies ρ'' = (x² − 1)ρ.
- `quantumPotential_gaussian` — For the Gaussian amplitude the quantum potential is the harmonic-oscillator expression Q(x) = −(ħ²/2m)(x² − 1).
- `quantumHJ_freeParticle` — The free-particle phase S(t,x) = px − p²t/(2m) solves the quantum Hamilton–Jacobi equation with vanishing classical and quantum potentials.
- `norm_normalize` — Normalizing a nonzero vector produces a unit vector; this is the content of the **ME-060** state update |ψ⟩ ↦ Ω̂|ψ⟩ / √⟨ψ|Ω̂†Ω̂|ψ⟩.
- `dyad_norm_one` — **ME-066** — the normalized dyadic cognition state Ψ_dyad = N(Ψ_H + Ψ_A + λ Ψ_H⊗Ψ_A) is a unit vector whenever the unnormalized combination is nonzero.

**`RequestProject/EFMW/ScalarField.lean`**

- `EFMWScalarEq_iff_expanded` — **ME-005 is exactly ME-002 rewritten with the flat-space expansion ME-004.**
- `EFMWScalarEq_iff_wave` — Equivalent single-coefficient form: the EFMW scalar equation is a wave equation whose time coefficient is (1 − α²)/c².
- `hasDerivAt_planeWave_time`
- `deriv_planeWave_time`
- `dtt_planeWave`
- `hasDerivAt_planeWave_space`
- `deriv_planeWave_space`
- `dxx_planeWave`
- `planeWave_solves_iff` — **Dispersion relation for the EFMW scalar equation.** A plane wave with nonzero amplitude solves the source-free EFMW scalar equation exactly when (1 − α²)ω² = c²k².
- `planeWave_phase_speed` — The EFMW scalar equation propagates plane waves at speed c/√(1−α²): for α² < 1 and k > 0, the admissible positive frequency is ω = ck/√(1−α²).
- `normSq_polarField` — **ME-017** — the probability density of the polar field is ρ².
- `wrightTensor_eq_scalarStress_add_ricci` — The informational tensor is exactly the scalar stress tensor plus the Ricci tensor; this is the precise sense in which ME-006 is "ME-015 plus recursive informational s…
- `modifiedEinstein_iff_unity` — **ME-008 is ME-007 with ME-006 substituted**; the two are equivalent.
- `modifiedEinstein_kappa_zero` — With κ = 0 the EFMW-modified Einstein equation reduces exactly to the standard Einstein equation: the framework is a conservative extension in this parameter.
- `maxwellLagrangian_neg` — The Maxwell Lagrangian is quadratic: reversing the sign of the field strength leaves it unchanged.

**`RequestProject/EFMW/Synthesis.lean`**

- `is`
- `unity_signature_universally_satisfiable` — **ME-001** — EFMW = F(φ, R, C, Ω).
- `unity_signature_two_distinct_functionals` — Contrast with ME-102: once F is pinned down to a concrete monitoring claim, the framework does make refutable predictions.
- `no_warning_at_perfect_coherence` — **Cross-sector consistency (ME-027, ME-028, ME-047).** If the self-model reproduces both the state and its rate of change, and the recursive-closure term is nonnegativ…
- `tracking_implies_asymptotic_coherence` — If the self-model converges to the state, the ME-047 coherence score converges to its maximum value 1.
- `selfModel_coherence_tendsto_one` — Concretely, the ME-023 self-model tracking law drives the ME-047 coherence score to 1.

**`RequestProject/EFMW/Systems.lean`**

- `leadTime_pos_iff`
- `warningUtility_nonneg`
- `warningUtility_mono_lead` — Warning utility increases with lead time (for admissible false-alarm rates and positive compute cost).
- `warningUtility_antitone_far` — Warning utility decreases as the false-alarm rate grows.
- `basinFraction_nonneg`
- `basinFraction_le_one`
- `closurePair_bijective` — Recursive closure preserves bijectivity: if the observer and the system maps are bijections, then so is every stage of the mutual recursion.
- `logos_recursion_unique` — **ME-064** — the LOGOS recursion L_{n+1} = C[L_n, O(L_n), M_n] is a well-founded definition: for any update rule and initial state there is exactly one trajectory.
- `chronoLogos_reversible` — **ME-073** — reversibility: an evolution family valued in bijections is inverted by its negative-time member.
- `chronoLogos_involution_iff` — **ME-074** — the involution condition T⁻¹ U T = U⁻¹ holds exactly when conjugation by the time-reversal operator inverts the evolution.
- `evidenceStep_iterate`
- `confidenceStep_lt_iff` — Confidence increases only when evidence exceeds error.
- `legalCoherence_eq_zero_iff` — The legal coherence functional collapses if any factor is absent.
- `constitutional_argmax_exists` — **ME-097** — the constitutional constraint A(x) = argmax[Benefit − Harm] is well posed over a finite nonempty action set.
- `accept_satisfiable` — An accepting outcome exists: the criterion is satisfiable.
- `accept_falsifiable` — A refuting outcome exists: the criterion is falsifiable — it is not automatically met.
- `accept_requires_replication` — Each clause is individually necessary: failing replication alone already blocks acceptance, even with a perfect lead time.
- `accept_mono` — Acceptance is monotone in the evidence: improving the lead time, lowering the false-alarm rate and lowering the compute cost cannot turn an accepted pilot into a rejec…

## Codex-888 (55)

**`Audit.lean`**

- `declarations`

**`Codex888/Dynamics.lean`**

- `integrate_zero`
- `integrate_add`
- `transmute_zero_steps`
- `transmute_without_ethics`
- `transmute_without_memory`
- `transmute_successor`
- `transmute_unit_fields` — Constant nonzero fields grow linearly: recursion alone does not imply stability.
- `integrate_prefix` — Prefix agreement suffices: later samples cannot change an earlier result.
- `evolve_eq_transmute`
- `fullProduct_without_ethics`

**`Codex888/Foundation.lean`**

- `rotate_zero`
- `rotate_add`
- `rotate_cycle`
- `rotations_commute`
- `rotate_inverse` — Undo any cyclic phase shift, including shifts greater than the base.
- `tensor2_cells`
- `tensor3_cells`

**`Codex888/Policy.lean`**

- `gate_accepts_iff`
- `gate_rejects_iff`
- `gate_sound`
- `run_approvals` — Every request in a successful trace passed its consent/ethics/threshold checks.
- `run_preserves` — Prefix preservation and clock monotonicity compose across arbitrary finite traces.
- `run_coherent`
- `run_memory_length`

**`Codex888/Registers.lean`**

- `registers_length`
- `registers_complete`
- `phases_nodup`
- `registers_nodup`
- `address_count` — Precisely 888^888 distinct, exhaustively enumerated symbolic registers.

**`Codex888/Symbolic.lean`**

- `fullTransformation_contains_all`
- `transmuteIdentity_contains_ethics`
- `tensor_contains_ethics`
- `tensor_signed_difference`

**`RequestProject/Codex888.lean`**

- `factorization_888`
- `address_space_card` — Assigning one of 888 base states to each of 888 positional axes gives 888 ^ 888 configurations: the Codex's "address space".
- `address_space_decimal_digits` — The address space 888 ^ 888 is a 2619-digit decimal number.
- `address_space_bits` — 2 ^ 8697 < 888 ^ 888 ≤ 2 ^ 8698: the address space carries between 8697 and 8698 bits, so it would take 8698 qubits to index it.
- `qudit_register_finrank` — The state space of a register of m qudits with d levels each, written in the computational basis indexed by the configurations Fin m → Fin d, has complex dimension d ^ m.
- `codex_register_finrank` — In particular, 888 qudits with 888 levels each span a Hilbert space of dimension 888 ^ 888.
- `rotational_symmetries_card` — There are exactly 888 complex 888-th roots of unity ("rotational symmetries").
- `rotational_symmetries_cyclic` — They form a cyclic group.
- `omega_isPrimitiveRoot`
- `omega_pow_n`
- `omega_pow_mod`
- `norm_omega`
- `iterate_shift`
- `iterate_clock`
- `shift_pow_n` — Applying the shift n times is the identity: X ^ n = 1.
- `clock_pow_n` — Applying the clock n times is the identity: Z ^ n = 1.
- `clock_shift_commutation` — The Weyl commutation relation Z X = ω X Z.
- `shift_norm_sq` — The shift operator is unitary (it preserves the total probability ∑ |ψ j|²).
- `clock_norm_sq` — The clock operator is unitary (it preserves the total probability ∑ |ψ j|²).
- `codex_weyl_relations` — For the Codex's 888-level system: X ^ 888 = Z ^ 888 = 1 and Z X = ω X Z with ω = exp (2πi / 888).
- `path_phase_norm` — In the Codex's path-integral expression ∫ Ψₑ ℜₑ Φₘ e^(i 𝓢ᵣ / Ξ) Dx, the phase factor has modulus one whenever the action S and the coherence parameter Ξ are real.

## Coherence-Prediction-Engine (17)
*Note: reference copies of FieldSpace / metrics files.*

**`references/FIELDSPACE_VERIFIED.lean`**

- `triplets_card` — FS-T01: there are 165 triplets.
- `sector_incidence` — FS-T02: every sector lies in exactly 45 triplets.
- `pair_incidence` — FS-T03: every pair of distinct sectors lies in exactly 9 triplets.
- `class_counts` — FS-T04: the six-class decomposition 56 + 56 + 28 + 16 + 8 + 1 = 165.
- `classes_exhaustive` — The six classes exhaust the atlas.
- `statement_inventory` — FS-T05: the inventory 45 + 90 + 90 + 360 = 585.
- `ablation` — FS-T06: deleting a set D of k sectors leaves C(11-k,3) triplets, all of which are exactly the triplets of the remaining sectors (closure under vertex deletion).
- `overlap_spectrum` — FS-T07: overlap spectrum of unordered pairs of distinct triplets (sharing 2 / 1 / 0 sectors): 1980 + 6930 + 4620 = 13530.
- `bilinear_reciprocity`

**`references/metrics.lean`**

- `coherenceScore_laws` — ME-047 law: for ε > 0 the score lies in [0, 1], is symmetric in x, m, and equals 1 exactly when the self-model matches the state (x = m).
- `recursiveIntegrity_laws` — ME-048 law: 0 ≤ I_rec ≤ C ≤ 1; integrity never exceeds state coherence.
- `kuramoto_laws` — ME-091 law: 0 ≤ K ≤ 1, and K = 1 for perfect phase locking.
- `kl_nonneg` — ME-092 law (Gibbs' inequality): for probability vectors p, q with q > 0, D_KL(P‖Q) = Σ p log(p/q) ≥ 0.
- `phraseEntropy_bounds` — ME-034 law: 0 ≤ H ≤ log n for any probability vector on n phrases (the upper bound follows from Gibbs' inequality against the uniform distribution).
- `collapseProb_distribution` — ME-061 law (Born compatibility): whenever some amplitude is non-zero, the collapse probabilities are non-negative and sum to 1.
- `collapseOmega_exists` — ME-059 law: on any finite, non-empty set of candidate outcomes s, the Collapse-Ω selection argmin_s [−ln P(s|ψ) + λ D(s, Φ) − γ R(s)] is well defined (a minimiser exis…
- `recursiveRisk_laws` — ME-089 law: with P(H), C ∈ [0, 1], risk lies in [0, P(H)], and is monotonically non-increasing in coherence C.

## EFMW-Axioms (12)

**`EFMWAxioms/Axioms.lean`**

- `A1_residual_limit_nonzero`
- `A2_trajectory_bounded`
- `A3_information_time_independent`
- `A4_rescaling_invariant`
- `A5_coupling_symmetric`
- `A6_all_points_related`
- `C7_quantum_generator_from_curvature`
- `C8_mass_is_potential_derivative`
- `C9_uncertainty_has_lower_bound`
- `C10_interface_matches`
- `C11_one_lattice_period`
- `C12_two_feedback_steps_remain_admissible`

## EFMW-Constants-Problem (5)

**`EFMWConstants/Core.lean`**

- `alpha_mul_denom_eq_e_sq`
- `maxwell_rearranged`
- `planck_length_time_relation`
- `generates_iff`
- `integer_ratio_generates` — If a supplied integer pair has the target ratio, the toy generator returns that target.

## EFMW_Post156_Zoo_Audit (30)

**`EFMWPost156Audit/DerivedCandidates.lean`**

- `phaseSpeed_neg` — T177: scalar phase speed cannot distinguish the sign of alpha.
- `real_wave_admissibility` — T178: a nontrivial real plane-wave dispersion solution forces alpha^2 < 1.
- `phaseSpeed_inversion` — T179: exact model speed can be inverted to recover alpha^2.
- `friedmann_rotation_sign_degeneracy` — T180: the current Friedmann extension cannot distinguish rotation sign.
- `friedmann_rotation_curvature_degeneracy` — T181: constant residual rotation is algebraically degenerate with curvature shift.

**`EFMWPost156Audit/FieldSpaceClosure.lean`**

- `mixedCurrent_null_slice` — A nontrivial construction satisfying all three required zero-amplitude slices.
- `mixedStress_pair_restriction`
- `mixedStress_chart_independent` — Different third-chart coefficients cannot affect the retained pair slice.
- `mixedCurrent_nontrivial`
- `zeroPaddedChart_shared_compatible`
- `zeroPaddedChart_not_gluingCompatible` — A concrete witness to the missing bridge, using two real source chart labels.
- `zeroPaddedChart_no_full_extension` — The generic gluing theorem cannot supply a full-vector extension of this zero-padded encoding, even though every shared-component comparison passes.
- `shared_compatibility_insufficient` — The shared-component predicate is strictly weaker than full-vector gluing.
- `vacuum_stress_overlap_iff` — On a removed scalar slice, the stress contains -g V(0).
- `vacuum_zero_required`

**`EFMWPost156Audit/ProjectedGluing.lean`**

- `projectedCompatible_iff_output_restriction` — The component predicate is exactly equality after restricting outputs too.
- `sum_mobius_component` — Boolean-lattice inversion with the equation label included in the bound.
- `IsComponentKBody.eq_sum_mobius`
- `projectedCompatible_of_restrictsTo` — Every projected global extension supplies the projected overlap condition.
- `exists_componentKBody_of_projectedCompatible` — Construct the extension by Möbius inversion, choosing for each component and support a containing chart that also contains the equation's own sector.
- `projected_atlas_gluing`
- `projected_atlas_gluing_unique` — Uniqueness holds in the stated component-indexed interaction class.
- `projected_full_vector_completion` — A compatible full-vector completion can be supplied after reconstruction.
- `fieldSpace_projected_atlas_gluing` — Repaired FS-C01 for the 165-chart atlas, with both restriction maps explicit.
- `zeroPaddedChart_has_unique_projected_extension` — The previously rejected full-vector example has a unique repaired extension.
- `repairedExample_restricts`
- `repair_preserves_full_vector_obstruction` — The repair is compatible with, and does not erase, the old negative result.
- `hiddenTriplet_is_three_body`
- `hiddenTriplet_projected_zero` — No triplet containing T can contain all three inputs of the hidden term.
- `ordinary_three_body_not_unique` — Ordinary three-body dependence alone cannot justify projected uniqueness.

## Einsteinian-156-Aristotle (72)

**`RequestProject/FieldSpace/Basic.lean`**

- `register`
- `card_sector`
- `mem_atlas`
- `atlas_card` — **FS-T01** (rank-3 projection count): the tripletAtlas has C(11,3) = 165 triplets.
- `sector_incidence` — **FS-T02** (uniform sector incidence): every sector lies in exactly C(10,2) = 45 triplets.
- `pair_incidence` — **FS-T03** (uniform pair incidence): every unordered pair of distinct sectors lies in exactly 9 triplets.
- `class_three_scalars` — **FS-T04** (six-class decomposition), class sizes.
- `class_one_gauge_two_scalars`
- `class_gravity_two_scalars`
- `class_gravity_gauge_scalar`
- `class_two_gauges_scalar`
- `class_gravity_two_gauges`
- `class_gravity_two_gauges_eq` — The unique gravity + two gauges triplet is {E, M, S}.
- `six_classes_partition` — **FS-T04** (exhaustiveness): every triplet lies in exactly one of the six classes, so the six classes partition the tripletAtlas.
- `ablate_eq` — Deleting sectors leaves exactly the complete 3-uniform hypergraph on the remaining sectors.
- `ablate_card` — **FS-T06**: removing any k sectors leaves C(11-k, 3) triplets.
- `ablate_card_one`
- `ablate_card_two`
- `ablate_card_three`
- `distinctPairs_card`
- `overlapPairs_two`
- `overlapPairs_one`
- `overlapPairs_zero`
- `overlap_le_two` — Two distinct triplets share at most two sectors, so overlaps 0, 1, 2 are exhaustive.
- `overlap_spectrum` — **FS-T07**: the overlap classes 2, 1, 0 exhaust all C(165,2) = 13530 unordered pairs of distinct triplets.

**`RequestProject/FieldSpace/Conservation.lean`**

- `contDiff_pd`
- `differentiable_pd`
- `pd_comm` — Equality of mixed partial derivatives (Schwarz) for C² functions.
- `pd_neg`
- `pd_sum`
- `div_div_antisymm` — The divergence of the divergence of an antisymmetric C² tensor vanishes identically: ∂_ν ∂_μ F^{μν} = 0.
- `pd_scalar_current`
- `scalar_current_constraint` — **FS-C03 (conservation closure), scalar-current form.** Suppose a gauge field strength F^{μν} (antisymmetric, C²) obeys a source-style gauge equation ∂_μ F^{μν} = κ φ …
- `scalar_current_extra_equation` — Combining with the scalar equation □φ + m² φ + s = 0 (where s stands for the remaining source terms, e.g. λ F_{αβ} F^{αβ}), every solution of the coupled system must a…
- `pd_coord`
- `linear_profile_obstruction` — A concrete instance of the obstruction.

**`RequestProject/FieldSpace/Coupling.lean`**

- `trilinear_null_slice` — **FS-T08** (trilinear null-slice law): the three-way term vanishes as soon as either participating field vanishes, so the three-way coefficient has no effect on the re…
- `restrict_third_zero` — Restricting to the slice φ_k = 0 leaves the i–j pair residual.
- `restrict_second_zero` — Restricting to the slice φ_j = 0 leaves the i–k pair residual.
- `shared_pair_overlap_consistency` — **FS-T09** (shared-pair overlap consistency): two triplets {i,j,k} and {i,j,l} with the same base term and the same i–j coefficient give the same residual for φ_i on t…
- `shared_pair_overlap_iff` — Conversely, the gluing condition is necessary: if the two restricted residuals agree for all values of φ_j (as polynomial functions), then the base terms and the pair …
- `triple_ablation_difference` — Removing the three-way term changes the residual by exactly that term.

**`RequestProject/FieldSpace/Gluing.lean`**

- `restrict_restrict`
- `restrict_of_subset`
- `restrict_of_superset`
- `mobius_congr`
- `mobius_insert`
- `sum_mobius_powerset`
- `mobius_eq_zero_of_not_subset`
- `sum_mobius_le`
- `mobius_sum`
- `IsKBody.eq_sum_mobius` — A k-body theory is recovered from its restrictions to sector subsets of size at most k by Möbius inversion.
- `gluingCompatible_of_restrictsTo` — Restrictions of any single global theory satisfy the gluing law.
- `exists_kBody_of_gluingCompatible` — A family satisfying the gluing law is the family of restrictions of a global k-body theory.
- `atlas_gluing` — **FS-C01 (existence).** For k ≤ |ι|, a family of local equations on the k-element charts satisfies the gluing law if and only if it consists of the chart restrictions …
- `atlas_gluing_unique` — **FS-C01 (uniqueness).** For k ≤ |ι|, a global k-body theory is determined by its restrictions to the k-element charts.
- `fieldSpace_atlas_gluing` — **FS-C01 for the FieldSpace atlas.** A family of local equations on the 165 triplets satisfies the gluing law if and only if it is the family of triplet restrictions o…

**`RequestProject/FieldSpace/Inventory.lean`**

- `sourceBlocks_heading_nodup` — Every block heading names three distinct sectors.
- `sourceBlocks_triplets_nodup` — The source headings are pairwise distinct triplets.
- `sourceBlocks_triplets_eq_atlas` — The source headings are exactly the 165 triplets of the complete atlas.
- `sourceBlocks_follow_grammar` — Every block of the source contains exactly the statements prescribed by the grammar.
- `source_inventory` — **FS-T05** (statement inventory) for the restored source file: 45 Einstein, 90 gauge-dynamical, 90 Bianchi and 360 scalar statements, 585 in total.
- `expected_inventory` — **FS-T05**, grammar-level version: summing the prescribed statement counts over the complete atlas gives 585, independently of the source file.
- `source_sector_incidence` — Every sector heads exactly 45 blocks in the source file.

**`RequestProject/FieldSpace/Reciprocity.lean`**

- `hasDerivAt_quadratic`
- `eq_of_hasDerivAt_affine`
- `potential_eq_x`
- `potential_eq_y`
- `reciprocal_of_potential` — A potential forces reciprocity.
- `masterPotential_isPotential` — Reciprocal couplings come from a potential, namely masterPotential.
- `exists_potential_iff_reciprocal` — **FS-C02** (master-action reciprocity), for a three-scalar triplet: the non-derivative parts of the three scalar equations are the partial derivatives of a single pote…
- `scalar_parameter_economy` — Counting: 56 directional pair symbols and 168 three-way symbols in the source, versus 28 unordered pairs and 56 triplets once reciprocity identifies them: 224 paramete…

## Emergentology (5)

**`Emergentology/Core.lean`**

- `fixed_point_stays`
- `wright_zero_weights`
- `wright_additive_in_coherence`
- `wright_entropy_penalty`
- `above_threshold_mono`

## FieldSpace (24)

**`FieldSpace/Ablations.lean`**

- `remove_one_remaining`
- `remove_two_remaining`
- `remove_three_remaining`
- `remove_one_deleted`
- `remove_two_deleted`
- `remove_three_deleted`

**`FieldSpace/Coupling.lean`**

- `restrict_third_zero` — Removing the third field kills both terms that require that field.
- `restrict_second_zero` — Removing the second field gives the symmetric reduction.
- `trilinear_null_slice_left` — A genuinely mixed trilinear contribution is invisible on either null slice.
- `trilinear_null_slice_right`
- `shared_pair_overlap_consistency` — Two triplet charts that share the same base term and i-j pair coefficient glue exactly on the slice where their respective third fields vanish.
- `triple_ablation_difference` — Triple-term ablation is exact subtraction of that term.

**`FieldSpace/Structure.lean`**

- `triplet_count` — Complete rank-3 atlas size.
- `fixed_sector_incidence` — Number of triplets containing a fixed sector.
- `fixed_pair_incidence` — Number of triplets containing a fixed unordered sector pair.
- `scalar_triples`
- `one_gauge_two_scalars`
- `gravity_two_scalars`
- `gravity_gauge_scalar`
- `two_gauges_scalar`
- `gravity_two_gauges`
- `class_partition` — The six structural classes exhaust the complete atlas.
- `statement_inventory` — Expected displayed-statement inventory for a fully populated atlas.
- `overlap_spectrum` — Pair-of-triplet overlap counts sum to all unordered pairs of distinct triplets.

## Monlithic_EFMW_102_Lean4 (2)

**`Catalog.lean`**

- `catalog_count`

**`Formalized.lean`**

- `scalar46_eq_scalar23_sq`

## Monolithic-102-Zoo-Lean4 (35)

**`Monolithic102/Catalog.lean`**

- `catalog_count`

**`Monolithic102/Formalized.lean`**

- `zero_gain_preserves_model`
- `int_pow_add`
- `int_pow_two`
- `scalar46_eq_scalar23_sq`
- `zero_gain_preserves_memory`
- `full_coherence_zero_risk`
- `zero_coherence_preserves_evidence`
- `zero_gain_preserves_identity`
- `acceptance_requires_baseline`
- `acceptance_requires_false_alarm`
- `acceptance_requires_compute`
- `acceptance_requires_replication`
- `no_acceptance_without_replication`
- `zero_regularizers`

**`Monolithic102/ZooAudit.lean`**

- `zooAudit_count`

**`legacy-mathlib/TURTLE-survivors/CollapseOmega.lean`**

- `omega_zero_regularizers`
- `divergence_scaling_algebra`

**`legacy-mathlib/TURTLE-survivors/Contraction.lean`**

- `discrete_fixed_point`
- `discrete_difference`
- `perturbation_propagation`

**`legacy-mathlib/TURTLE-survivors/Evaluation.lean`**

- `acceptance_requires_baseline`
- `acceptance_requires_false_alarm`
- `acceptance_requires_compute`
- `acceptance_requires_replication`
- `no_acceptance_without_replication`
- `regeneration_preserves_invariant`

**`legacy-mathlib/TURTLE-survivors/Exponent.lean`**

- `pow_two_mul`
- `pow_46_eq_pow_23_sq`

**`legacy-mathlib/TURTLE-survivors/Potential.lean`**

- `negative_potential_derivative_eq_dynamics`
- `gradient_bridge`
- `approximate_gradient_bridge`

**`legacy-mathlib/TURTLE-survivors/Robustness.lean`**

- `alarm_translation_invariant`
- `equal_score_not_state_equality`
- `multiplicative_gate_zero_left`

## Monolithic-Zoo-Lean4 (98)

**`Ant.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`Axolotl.lean`**

- `acceptable_retains_invariants`

**`Bat.lean`**

- `placebo_has_priority`

**`Beaver.lean`**

- `accepted_requires_rollback`
- `accepted_requires_bounds`

**`Bison.lean`**

- `queue_bounded`

**`Bonobo.lean`**

- `mutual_gain_excludes_loser`

**`Butterfly.lean`**

- `run_records_initial_and_steps`

**`Cat.lean`**

- `positive_removal_hurt`
- `removal_hurts_iff`

**`Chameleon.lean`**

- `excess_nonnegative`
- `expected_explains`

**`Cobra.lean`**

- `nonimproving_proxy_zero`

**`Core.lean`**

- `admissible_no_leakage`
- `not_admissible_if_unfrozen`
- `rankScores_length`
- `firstIndex_nil`
- `hasVeto_cons`
- `memoryNumerator_sign`
- `memoryNumerator_zero`

**`Crab.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`Crocodile.lean`**

- `common_shift_cancels`
- `causal_requires_design`

**`Dolphin.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`Dragon.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`Eagle.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`Elephant.lean`**

- `current_members_active`
- `zero_fuel_stops`

**`Falcon.lean`**

- `positive_margin_iff_on_time`
- `absent_alarm_no_timing`

**`Fox.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`Gecko.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`Hedgehog.lean`**

- `heldout_not_development`

**`Hive.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`Horse.lean`**

- `handoff_retains_uncertainty`

**`Jellyfish.lean`**

- `node_count_preserved`

**`Lynx.lean`**

- `emergent_requires_replication`

**`Magpie.lean`**

- `no_history_no_alarm`

**`Mantis.lean`**

- `unready_calibrates`

**`Mole.lean`**

- `no_indicators_no_failure_claim`

**`Moth.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`Octopus.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`Orca.lean`**

- `complete_requires_ack`

**`Owl.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`Penguin.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`Phoenix.lean`**

- `stable_requires_every_checkpoint`

**`Pulse.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`Raven.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`Registry.lean`**

- `exactly_forty_six`
- `no_duplicate_animals`
- `names_match_count`

**`Rhino.lean`**

- `survives_selected_invariant`

**`Salmon.lean`**

- `exhaustion_not_origin`

**`Shark.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`Shepherd.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`Spider.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`Termite.lean`**

- `population_preserved`

**`Tortoise.lean`**

- `split_reconstructs`
- `train_precedes_test`

**`Turtle.lean`**

- `applicable_veto_blocks_support`
- `empty_is_insufficient`

**`Weasel.lean`**

- `retained_within_budget`

**`Whale.lean`**

- `empty_history_zero_gap`

**`Wolf.lean`**

- `alarm_requires_distributed_support`

## Monolithic_Zoo_Run (19)
*Note: same files as `Monolithic-102-Zoo-Lean4/legacy-mathlib/TURTLE-survivors`.*

**`CollapseOmega.lean`**

- `omega_zero_regularizers`
- `divergence_scaling_algebra`

**`Contraction.lean`**

- `discrete_fixed_point`
- `discrete_difference`
- `perturbation_propagation`

**`Evaluation.lean`**

- `acceptance_requires_baseline`
- `acceptance_requires_false_alarm`
- `acceptance_requires_compute`
- `acceptance_requires_replication`
- `no_acceptance_without_replication`
- `regeneration_preserves_invariant`

**`Exponent.lean`**

- `pow_two_mul`
- `pow_46_eq_pow_23_sq`

**`Potential.lean`**

- `negative_potential_derivative_eq_dynamics`
- `gradient_bridge`
- `approximate_gradient_bridge`

**`Robustness.lean`**

- `alarm_translation_invariant`
- `equal_score_not_state_equality`
- `multiplicative_gate_zero_left`

## MultiValuedClassicalAction-Lean4 (2)

**`MultiValuedClassicalAction.lean`**

- `certificate_has_normalization` — Logical sanity check: a reconstruction certificate only certifies the assumptions explicitly contained in it.
- `reconstruction_with_anticircularity` — Anti-circularity remains a separate obligation; it cannot be obtained merely from a reconstruction certificate.

## Nightengale-Full-Zoo-Audit (98)
*Note: copy of the `Monolithic-Zoo-Lean4` animal files.*

**`lean-source/Ant.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`lean-source/Axolotl.lean`**

- `acceptable_retains_invariants`

**`lean-source/Bat.lean`**

- `placebo_has_priority`

**`lean-source/Beaver.lean`**

- `accepted_requires_rollback`
- `accepted_requires_bounds`

**`lean-source/Bison.lean`**

- `queue_bounded`

**`lean-source/Bonobo.lean`**

- `mutual_gain_excludes_loser`

**`lean-source/Butterfly.lean`**

- `run_records_initial_and_steps`

**`lean-source/Cat.lean`**

- `positive_removal_hurt`
- `removal_hurts_iff`

**`lean-source/Chameleon.lean`**

- `excess_nonnegative`
- `expected_explains`

**`lean-source/Cobra.lean`**

- `nonimproving_proxy_zero`

**`lean-source/Core.lean`**

- `admissible_no_leakage`
- `not_admissible_if_unfrozen`
- `rankScores_length`
- `firstIndex_nil`
- `hasVeto_cons`
- `memoryNumerator_sign`
- `memoryNumerator_zero`

**`lean-source/Crab.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`lean-source/Crocodile.lean`**

- `common_shift_cancels`
- `causal_requires_design`

**`lean-source/Dolphin.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`lean-source/Dragon.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`lean-source/Eagle.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`lean-source/Elephant.lean`**

- `current_members_active`
- `zero_fuel_stops`

**`lean-source/Falcon.lean`**

- `positive_margin_iff_on_time`
- `absent_alarm_no_timing`

**`lean-source/Fox.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`lean-source/Gecko.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`lean-source/Hedgehog.lean`**

- `heldout_not_development`

**`lean-source/Hive.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`lean-source/Horse.lean`**

- `handoff_retains_uncertainty`

**`lean-source/Jellyfish.lean`**

- `node_count_preserved`

**`lean-source/Lynx.lean`**

- `emergent_requires_replication`

**`lean-source/Magpie.lean`**

- `no_history_no_alarm`

**`lean-source/Mantis.lean`**

- `unready_calibrates`

**`lean-source/Mole.lean`**

- `no_indicators_no_failure_claim`

**`lean-source/Moth.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`lean-source/Octopus.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`lean-source/Orca.lean`**

- `complete_requires_ack`

**`lean-source/Owl.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`lean-source/Penguin.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`lean-source/Phoenix.lean`**

- `stable_requires_every_checkpoint`

**`lean-source/Pulse.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`lean-source/Raven.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`lean-source/Registry.lean`**

- `exactly_forty_six`
- `no_duplicate_animals`
- `names_match_count`

**`lean-source/Rhino.lean`**

- `survives_selected_invariant`

**`lean-source/Salmon.lean`**

- `exhaustion_not_origin`

**`lean-source/Shark.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`lean-source/Shepherd.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`lean-source/Spider.lean`**

- `output_length`
- `valid_column_count`
- `report_requires_freeze`

**`lean-source/Termite.lean`**

- `population_preserved`

**`lean-source/Tortoise.lean`**

- `split_reconstructs`
- `train_precedes_test`

**`lean-source/Turtle.lean`**

- `applicable_veto_blocks_support`
- `empty_is_insufficient`

**`lean-source/Weasel.lean`**

- `retained_within_budget`

**`lean-source/Whale.lean`**

- `empty_history_zero_gap`

**`lean-source/Wolf.lean`**

- `alarm_requires_distributed_support`

## Universal-Cognitive-Attractor (3)

**`UCA/Core.lean`**

- `fixed_iterate`
- `reaches_fixed_stays`
- `population_target_reached`

## papers (7)

**`formal/efmw-local-repair/Core.lean`**

- `repairStep_locallyDetermined`
- `repairStep_fixed_iff_residual_zero`
- `fixedPoint_unique`
- `iterateN_distance_bound`
- `iterateN_converges_of_geometric_decay`
- `swapPair_two_cycle`
- `identityPair_has_two_fixed_points`

