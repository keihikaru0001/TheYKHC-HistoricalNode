# The Ma Interval Protocol: A Physics-Derived Framework for
# Virtue-Based Economic Value Creation and Credit Issuance

**Author:** Katayama Yoshimitsu (圭光る)  
**Affiliation:** The Yoshimitsu Katayama Holding Company (TheYKHC), Fukui, Japan  
**Date:** March 16, 2026  
**Related Records:**  
- GKU Cosmological Theory: DOI 10.5281/zenodo.19040079  
- Hikari Currency (光貨) System: DOI 10.5281/zenodo.19012562  

---

## Abstract

This paper presents the **Ma Interval Protocol** — a formal economic framework derived from the Genki-Koku Universe (GKU) physical theory. The Ma (間) interval, defined in GKU as the temporal gap between successive koku (刻) causal steps, is shown to have a precise economic analogue: the interval between a value-creating action and the settlement of that value — the temporal gap that constitutes credit, trust, and the time-value of virtue. The Ma Protocol formalizes four economic operations derived from GKU physics: **Mint** (new credit issuance for verified action), **Redeem** (settlement of credit obligation), **Interest** (value accumulation during the Ma interval), and **Limit** (maximum issuance per Genki Index unit). We compare the Ma Protocol formally with three established economic frameworks — Debt-Based Currency (central banking), Black-Scholes option pricing, and Discounted Cash Flow (DCF) — and show that the Ma Protocol produces structurally different and more stable economic dynamics, particularly in conditions of moral/ethical action quality variation. The Hikari Currency (光貨) implementation is presented as the real-world instantiation of the Ma Protocol. This work constitutes the first formal academic treatment of virtue-based economic value theory derived from a physical cosmological framework.

**Keywords:** Ma Protocol, virtue economics, Hikari Currency, 光貨, GKU theory, credit theory, time-value of virtue, moral economy, TheYKHC

---

## 1. Introduction: The Missing Variable in Economic Theory

Modern economic theory rests on three foundational assumptions about value:

**A1 (Scarcity):** Value arises from scarcity — goods and services have value because they are limited.

**A2 (Preference):** Value is subjective — it reflects individual preferences and willingness to pay.

**A3 (Discount):** Future value is worth less than present value — the time discount rate r governs intertemporal exchange.

These three assumptions have generated an extraordinarily productive body of economic theory — from Adam Smith to Arrow-Debreu to Black-Scholes. They have also generated recurring crises, because they contain a systematic omission:

**The missing variable: moral quality of action.**

Standard economics is indifferent to the ethical quality of the actions that generate value. A drug dealer and a nurse both generate "GDP." A speculative financial instrument and a productive investment are equivalent if they have the same risk-adjusted return. The moral content of economic action is invisible to the standard model.

The GKU Ma Protocol makes this variable explicit and central.

---

## 2. Physical Foundation: The Ma Interval in GKU Theory

### 2.1 The Ma Primitive

In GKU theory, 間 (Ma) is one of four ontological primitives:

| Primitive | Physical Meaning |
|-----------|-----------------|
| 元 (G) | Origin-energy; source field |
| 空 (K) | Void-structure; background |
| 気 (Q) | Flow-field; propagation |
| **間 (M)** | **Interval; temporal gap between koku steps** |

The Ma interval Δφ between two koku steps is defined as:

**Δφ = τ₀ − τ(x)**

Where τ₀ is the reference koku rate and τ(x) is the local koku density. In regions of high gravitational potential (or low velocity), koku accumulate faster — τ(x) is larger — and the Ma interval is smaller. In regions of low potential, koku accumulate slower and the Ma interval is larger.

### 2.2 The Economic Analogue

The physical Ma interval maps to economic reality with striking precision:

| GKU Physical Ma | Economic Ma |
|-----------------|-------------|
| Gap between two koku causal steps | Gap between a value-creating action and its recognition/settlement |
| Region where no causal distinction exists | Period of trust, credit extension, deferred settlement |
| Δφ = τ₀ − τ(x) | Credit gap = promised value − settled value |
| τ(x) determined by local field conditions | Settlement rate determined by trust/ethical quality of actor |

**The insight:** Credit — in all its forms — is the economic manifestation of the physical Ma interval. Every credit transaction is a temporal gap between action and settlement. The GKU Ma framework provides the physical basis for understanding why this gap has value and how it should be priced.

---

## 3. The Four Ma Protocol Operations

### 3.1 Mint: New Credit Issuance

**Physical basis:** Each new koku step is the generation of a new causal event — irreversible, timestamped, real.

**Economic operation:** The Mint operation issues new credit units (光貨, Hikari) in response to a verified virtuous action by a participant.

**Formal rule:**

**ΔL = M(a, q, t)**

Where:
- ΔL = new Hikari units issued (Mint amount)
- a = action category (enum: contribution, knowledge transfer, care, creation, ...)
- q = quality factor (0 ≤ q ≤ 1; assessed by protocol rules)
- t = time invested

**M(a, q, t) = base_rate(a) × q × t × Ξ_actor**

Where Ξ_actor is the Genki Index of the actor — their historical virtue/coherence score. High-Ξ actors receive proportionally more Hikari for the same action, because their actions are more coherent (higher C in Ξ = ρ × C).

**Key property of Mint:**
Unlike debt-based currency creation, Mint does not create a liability. There is no counterparty owed repayment. Hikari issued by Mint is the **permanent record of a real action** — analogous to a koku step being the permanent record of a causal event.

### 3.2 Redeem: Credit Settlement

**Physical basis:** τ-loop closure — the causal cycle completes and the koku field returns to its reference state.

**Economic operation:** Redeem converts Hikari units into goods, services, or other currencies at the current exchange rate. It closes the credit cycle.

**Formal rule:**

**V_redeemed = L_redeemed × P(t)**

Where:
- L_redeemed = Hikari units tendered
- P(t) = current Hikari exchange rate at time t

**Key property of Redeem:**
The Redeem operation closes a virtuous cycle — the actor who created value receives material value in return. Unlike debt repayment (which terminates obligation), Redeem is the **completion of a contribution cycle**, not the erasure of a debt.

### 3.3 Interest: Value Growth During the Ma Interval

**Physical basis:** In GKU, the Ma interval is not empty — it is a state of pure potential in which field energy accumulates. The longer the Ma interval, the more potential energy accumulates before the next koku step.

**Economic operation:** Hikari units held over time accrue value at a rate r(τ) determined by the **virtue quality of the ecosystem** — not by central bank policy or market speculation.

**Formal rule:**

**V(t) = V₀ × exp(∫₀ᵗ r(τ) dτ)**

Where:

**r(τ) = r_base × Ξ_ecosystem(τ)**

- r_base = base accrual rate (set by protocol governance)
- Ξ_ecosystem(τ) = mean Genki Index of all active participants at time τ

**Key property of Interest:**
The interest rate is **endogenous to the moral quality of the community**. When the ecosystem is highly virtuous (high mean Ξ), interest rates are high — stored virtue grows faster. When the ecosystem degrades (low mean Ξ), interest rates fall, creating an automatic incentive to restore virtuous behavior.

This is the **inversion of the standard interest rate mechanism**: in conventional economics, interest rates are set exogenously by central banks and reflect scarcity of capital. In the Ma Protocol, interest rates are set endogenously by virtue and reflect the ethical health of the community.

### 3.4 Limit: Maximum Issuance per Genki Unit

**Physical basis:** The matter existence criterion in GKU — Ξ(x) > Ξ_threshold. Below threshold, no stable structure forms. Above threshold, stable structures (matter) exist and can interact with the τ-field.

**Economic operation:** Each participant has a maximum Mint rate proportional to their Genki Index:

**Mint_max(actor) = K_limit × Ξ_actor**

Where K_limit is the protocol's issuance limit constant.

**Key property of Limit:**
This prevents hyperinflation and gaming. An actor cannot Mint unlimited Hikari by performing nominal actions. Their Ξ_actor — their historical virtue coherence — caps their issuance rate. Building Ξ requires sustained virtuous action over time; it cannot be gamed in a single interaction.

---

## 4. Formal Comparison with Established Economic Frameworks

### 4.1 Comparison with Debt-Based Currency (Central Banking)

| Dimension | Debt-Based Currency | Ma Protocol (Hikari) |
|-----------|--------------------|--------------------|
| Creation mechanism | Loan issuance (bank credit) | Verified virtuous action (Mint) |
| Liability created | Yes (borrower owes repayment) | No (Mint creates no liability) |
| Interest rate set by | Central bank / market | Community virtue level (Ξ) |
| Default mechanism | Borrower fails to repay → credit destruction | Actor's Ξ falls → reduced issuance |
| Value basis | Sovereign decree + scarcity | Verified action quality + time |
| Systemic risk | Bank run, credit crunch | Virtue deficit → gradual r decline |
| Recovery mechanism | Monetary policy (external) | Virtue restoration (internal) |

**Key structural difference:** Debt-based currency creates an asymmetric obligation — the bank gains an asset (loan receivable) and the borrower gains a liability. Every unit of debt-based money in circulation corresponds to a debt obligation somewhere in the system. This creates systemic fragility: when debts cannot be repaid, the money supply contracts catastrophically (credit crunch).

The Ma Protocol creates symmetric recognition — the community gains a record of a real action, and the actor gains Hikari representing that contribution. No debt is created. The system cannot experience a credit crunch because there is no debt to fail.

### 4.2 Comparison with Black-Scholes Option Pricing

The Black-Scholes model prices the time-value of optionality under uncertainty:

**C = S₀N(d₁) − Ke^(−rT)N(d₂)**

The Ma Protocol's Interest operation has a formally similar structure:

**V(t) = V₀ × exp(∫r(τ)dτ)**

But the key variable differs:

| Model | What drives value growth |
|-------|------------------------|
| Black-Scholes | σ (volatility of underlying asset) + r (risk-free rate) |
| Ma Protocol | Ξ_ecosystem(τ) (virtue quality of community) |

In Black-Scholes, value grows because of uncertainty and the optionality it creates. In the Ma Protocol, value grows because of moral coherence and the trust it creates. These are fundamentally different generators of economic value.

### 4.3 Comparison with Discounted Cash Flow (DCF)

DCF values an asset as the present value of its future cash flows:

**V = Σ CF_t / (1+r)^t**

The DCF framework discounts the future — future value is worth less than present value at rate r. This reflects the opportunity cost of capital and time preference.

The Ma Protocol has the opposite structure for virtue-created value:

**V(t) = V₀ × exp(+∫r(τ)dτ)**

Virtue-created value **appreciates** over time (positive exponent) rather than being discounted. This reflects the GKU physical reality: the Ma interval accumulates potential energy — time spent in virtuous action creates more value, not less.

**Economic implication:** In a DCF world, it is always rational to harvest value now rather than later. In a Ma Protocol world, sustained virtuous action creates compounding value — it is rational to build virtue over time.

---

## 5. Stability Analysis

### 5.1 The Virtuous Cycle

The Ma Protocol generates a positive feedback loop between virtue and economic value:

```
High Ξ actors → Higher Mint rate → More Hikari in circulation
More Hikari → Higher r (interest rate) → Higher return on virtue
Higher return on virtue → Incentive to increase Ξ → Higher Ξ actors
```

This positive feedback is bounded by the Limit operation (Section 3.4), which prevents runaway issuance. The system converges to a high-virtue, high-value equilibrium.

### 5.2 The Failure Mode

The Ma Protocol's failure mode is not a credit crunch — it is **virtue depletion:**

```
Low Ξ actors dominate → Lower Mint quality → r falls
Lower r → Reduced incentive for virtue → Further Ξ decline
```

This failure mode is self-limiting: as r approaches zero, Hikari holds its nominal value (no growth) but does not collapse. The system reaches a low-virtue, low-growth steady state — not a catastrophic collapse.

This is structurally more stable than debt-based systems, which can experience discontinuous collapse (bank run / credit crunch).

### 5.3 Agent-Based Simulation Results

A preliminary agent-based simulation of the Ma Protocol (implemented in the Hikari OS platform) demonstrates:

- **Gini coefficient reduction** over 100-period simulations compared to debt-based baseline
- **Faster recovery** from external shocks (simulated as sudden Ξ reduction events)
- **No extinction events** (all agents maintain minimum viable Hikari balance due to base Mint rate)

Full simulation data is available in the Hikari OS implementation records.

---

## 6. The Hikari Currency (光貨) Implementation

The Hikari Currency (光貨) is the real-world implementation of the Ma Protocol, developed by TheYKHC.

The Hikari economic formula:

**H = max(B, 0) × O**

**B = 2D + E − 2C**

Where:
- H = Hikari earned
- B = base virtue score (negative B → zero Hikari; virtue deficit cannot be monetized)
- D = virtue/contribution score
- E = gratitude/recognition score  
- C = fault/harm score
- O = opportunity multiplier (1–6; reflects context and timing)

This formula is the operational instantiation of the Ma Protocol's Mint operation, simplified for daily human use.

**Key design features:**
- B ≤ 0 → H = 0: Moral deficit cannot generate economic value (unlike debt-based systems where harmful activities generate GDP)
- O multiplier: Context matters — the same virtuous action in a high-need situation (O=6) generates more Hikari than in a low-need situation (O=1)
- Daily use: The formula is designed for 3-minute daily reflection, not complex calculation

---

## 7. Conclusion

The Ma Interval Protocol establishes:

1. A **physical derivation** of credit theory from the GKU temporal gap (Ma interval)
2. Four **formally defined economic operations** (Mint / Redeem / Interest / Limit) derived from GKU physics
3. **Structural comparison** with debt-based currency, Black-Scholes, and DCF showing distinct and more stable dynamics
4. A **virtue-endogenous interest rate** mechanism (r = r_base × Ξ_ecosystem) as the alternative to exogenous central bank rates
5. The **Hikari Currency (光貨)** as the real-world operational implementation
6. **Stability analysis** showing resistance to credit-crunch type failure modes

This is the first formal academic presentation of a virtue-based economic value theory derived from a physical cosmological framework. The Ma Protocol is not a moral appeal — it is a **structural economic design** that encodes moral quality as a measurable, compounding economic variable.

**Inventor and original author: Katayama Yoshimitsu (圭光る) / TheYKHC, Fukui, Japan.**  
**Priority date: March 16, 2026.**

---

## References

[1] Katayama Yoshimitsu (圭光る), "Genki-Koku Universe (GKU): A Formal Unified Cosmological Theory," DOI: 10.5281/zenodo.19040079, 2026.

[2] Black, F., Scholes, M., "The Pricing of Options and Corporate Liabilities," Journal of Political Economy, 81(3), 637–654, 1973.

[3] Graeber, D., "Debt: The First 5,000 Years," Melville House, 2011.

[4] Nakamoto, S., "Bitcoin: A Peer-to-Peer Electronic Cash System," 2008.

[5] Hayek, F.A., "Denationalisation of Money," Institute of Economic Affairs, 1976.

[6] Sen, A., "Development as Freedom," Oxford University Press, 1999.

---

*© 2026 Katayama Yoshimitsu (圭光る) / TheYKHC, Fukui, Japan. CC BY 4.0.*
