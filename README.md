# 📊 SaaS Pricing Elasticity & Tier Optimization Simulator

An interactive, strategic product management dashboard designed to model customer demand decay curves, evaluate price elasticity parameters ($E_d$), and calculate the mathematical "sweet spot" that maximizes monthly recurring revenues (MRR) and annual margins (ARR) across tiered subscription models.

### 🔗 Live Link: [Launch the Interactive Simulator Here](https://dhavalk21.github.io/saas-pricing-elasticity-optimizer/)


## 🌟 Core PM Competencies Demonstrated

* **Monetization & Packaging Strategy:** Understands how to structure multi-tier subscription packaging (e.g., Pro vs. Enterprise) and balance conversion shares to optimize weighted Average Revenue Per Paid User (ARPPU).
* **Price Elasticity Modeling:** Uses price elasticity coefficients ($E_d$) and exponential decay formulas to simulate demand changes, helping teams avoid ungrounded price increases.
* **Financial Forecasting & ROI Analysis:** Projects incremental ARR, monthly margins, and relative percentage lift from any packaging change, making the tool a valuable asset for CFO-level reviews.
* **Executive Decision Briefing:** Features a built-in automated briefing generator that translates complex elasticity calculations into clear, plain-English strategic recommendations.

## ⚙️ How the Math Works

This simulator uses continuous economic modeling to project user lifecycle value and growth:

1. **Exponential Demand Decay Curve:** To prevent unrealistic linear drops (where conversion rates drop to negative numbers), we use an exponential decay function to model conversion rate ($CR_{\mathrm{new}}$) relative to price adjustments:
   $$CR_{\mathrm{new}} = CR_0 \times e^{-k \cdot (P_{\mathrm{new}} - P_0)}$$
   *Where $k = E_d / P_0$ is the decay constant, $E_d$ is the Price Elasticity of Demand, and $P_{\mathrm{new}}$ is your new weighted ARPPU.*

2. **Weighted Average Revenue Per Paid User (ARPPU):** Combines subscription pricing and expected tier adoption shares:
   $$\text{ARPPU} = (P_{\mathrm{Pro}} \times \text{Pro Share} \%) + (P_{\mathrm{Ent}} \times \text{Enterprise Share} \%)$$

3. **Annual Recurring Revenue Projection (ARR):**
   $$\text{ARR}_{\mathrm{Projected}} = \text{Monthly Traffic} \times CR_{\mathrm{new}} \times \text{ARPPU} \times 12$$
---
&copy; 2026 Dhaval Kareliya. All rights reserved.
