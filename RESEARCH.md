# Research Statement & Agenda

**Focus:** On-Chain Security, Autonomous Financial Agents, and Verifiable Execution Constraints  
**Identity:** Independent Researcher & Systems Builder  

## 🎯 Primary Research Question
> *Which security properties of autonomous financial execution can be deterministically enforced at the on-chain execution boundary, and which inherently require pre-execution simulation, behavioral monitoring, or external verification?*

**Conceptual Foundation:** This question explores a fundamental boundary in agentic systems: *What can be made mathematically impossible by constraining execution, versus what can only be evaluated by understanding the proposed action before it occurs?* 

*(Alternate formulations guiding this work: "Once an agent has been granted authority to execute financial transactions, what properties of that authority can be enforced deterministically at the EVM execution boundary?")*

---

## 🔬 Supporting Research Pillars
To answer the primary question, my research is structured around four supporting pillars. These are not isolated projects, but interconnected lenses through which to evaluate autonomous financial safety:

1. **Property Identification & Granularity:**  
   Which specific security properties matter most for common operations (e.g., approvals, token transfers, DEX swaps, vault deposits/withdrawals), and how precisely must execution constraints define permitted actions to provide meaningful safety guarantees?
2. **Enforcement Boundaries:**  
   Which of these properties can existing standards (e.g., ERC-8004, ERC-8183, and proposed frameworks like ERC-8232) and smart contracts enforce directly at the EVM level, and under what specific conditions?
3. **Composability & Adversarial Failure Modes:**  
   How do safety guarantees break when transactions cross multiple contracts, protocols, or authorization paths? Specifically, how do adversarial transaction sequences expose gaps between an agent's intended policy and its actual on-chain execution?
4. **Reproducible Evaluation Methodology:**  
   How can these security properties be tested reproducibly across different enforcement architectures, independent of opaque off-chain oracles?

---

## ⚙️ Experimental Framework (Methodology)
I employ a **"build-to-evaluate"** research methodology. Rather than relying solely on theoretical modeling, I construct minimal, functional research environments ("labs") to stress-test hypotheses. 

Crucially, **my transaction tests are experiments, not research questions**. They are designed to probe the supporting pillars above. Current experimental vectors include:
- **Test 1:** Deterministic authority constraints on delegated spending limits.
- **Test 2:** Pre-execution simulation vs. direct on-chain enforcement of swap slippage.
- **Test 3:** Composability failure modes across multi-hop DeFi protocols.
- **Test 4:** Temporal and velocity limits (spending rates/call frequency) without behavioral monitoring.

*Artifacts mapping to this framework:*
- [`ai-agent-guardrail-lab`](https://github.com/neonmercenary/ai-agent-guardrail-lab): Prototyping the pre-execution filtering layer.
- [`snowgate`](https://github.com/neonmercenary/snowgate) & [`procurement_repo`](https://github.com/neonmercenary/procurement_repo): Implementing session-aware treasury firewalls and escrow-backed settlement.
- [`ERCs`](https://github.com/neonmercenary/ERCs): Exploring standardization boundaries for agentic commerce.

---

## 🔭 Current Open Questions & Future Directions
Following a review of existing literature on cross-layer security for on-chain agents, my immediate focus is narrowing the scope to identify a specific, unanswered gap. Current open directions include:
- **The Standardization Boundary:** What should a base standard (e.g., a proposed ERC-8232 for agent payments) strictly define, and what must remain optional or implementation-specific to avoid stifling innovation?
- **The Gas/State Cost Tradeoff:** What computational and storage overhead do deterministic execution constraints introduce, and at what point do they become economically unviable for everyday operations?

## 🤝 Collaboration & Contact
I am open to discussing research collaborations, peer review of my experimental frameworks, or opportunities to contribute to applied AI safety and blockchain security teams. 
- **GitHub:** [@neonmercenary](https://github.com/neonmercenary)
- **Email:** [benjamin.mgbeoji@financier.net]
- **Twitter/X / LinkedIn:** [https://x.com/secondfrontman]

---
*Last updated: October 2026*
