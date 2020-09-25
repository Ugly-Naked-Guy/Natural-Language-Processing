# Finite-State Transducers 有限状态转换器

A **finite-state transducer**  T = {Q, Σ, Δ, q0, F, δ, σ} consists of:
- A finite **set of states** Q = {q0, q1,.., qn}
- A finite alphabet Σ of **input symbols** (e.g. Σ = {a, b, c,...})
- A finite alphabet Δ of **output symbols** (e.g. Δ = {+N, +pl,...})
- A designated **start state** q0 ∈ Q
- A set of **final states** F ⊆ Q
- A **transition function** δ: Q × Σ → 2^Q
  δ(q,w) = Q’ for q ∈ Q, Q’ ⊆ Q, w ∈ Σ
- An **output function** σ: Q × Σ →Δ*
  σ(q,w) = ω for q ∈ Q, w ∈ Σ, ω ∈ Δ*
  If the current state is q and the current input is w, write ω.
  (NB: Jurafsky&Martin (2nd ed.) define σ: Q × Σ* → Δ*. Why is this equivalent?)
