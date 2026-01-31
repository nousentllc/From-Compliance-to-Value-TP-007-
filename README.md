# From Compliance to Value: Monetized Reliability Risk (TP-007)

**Authors:** Justin Candler & Uriel (Nous Enterprises LLC)  
**Date:** October 2025  
**Series:** Unified Energy Valuation Framework (UEVF), Technical Paper 007  

## 📖 Overview

The structural evolution of the North American power grid—driven by high-VRE penetration and massive AI load growth—has rendered traditional binary reliability metrics (like "1-in-10" LOLE) obsolete.

This repository contains the LaTeX source, mathematical proofs, and empirical baselines for **"From Compliance to Value,"** a policy and planning framework that transitions Resource Adequacy from a physical compliance exercise to an economic value optimization.

By coupling **Expected Unserved Energy (EUE)** with the **Value of Lost Load (VOLL)**, we derive a continuous, annualized cost of risk that allows transmission upgrades, battery storage, and demand response to compete on a level playing field.

## 🚀 Key Innovations

### 1. The Marginal Reliability Value (MRV)
We replace static capacity credits with a gradient-based valuation:
$$MRV_{\ell} = - \frac{\partial EUE}{\partial K_{\ell}} \times VOLL$$
This quantifies exactly how much *societal outage cost* is avoided by adding 1 MW of capacity at a specific location ($\ell$) under specific transmission constraints.

### 2. The "Dunkelflaute" Adjustment (Appendix B)
Standard models assume independent generator outages. We introduce a **Correlated Fuel Availability (CFA)** state variable to model the non-linear risk of coincident gas pipeline failures and low-wind events, revealing the "Hockey Stick" function of winter risk in MISO.

### 3. The AI / Large Load Denominator (Appendix C)
We derive the **Reliability Incidence Share (RIS)** for Hyperscale Data Centers. Unlike residential load ($LF \approx 0.45$), high-load-factor AI clusters ($LF \approx 0.95$) dilute reserve margins across all 8,760 hours, requiring a strictly higher "Reliability Adder" to remain revenue neutral to the system.

## 📂 Repository Contents

* **`From_Compliance_to_Value.tex`**: The primary source code for the technical report.
* **`references.bib`**: Curated bibliography of FERC orders, NREL studies, and UEVF technical series.
* **`figures/`**: Placeholder directory for reliability surface plots (EUE vs. Capacity).
* **`appendices/`**:
    * `Appendix_A_Two_Bus_Derivation.tex`: Mathematical proof of endogenous deliverability.
    * `Appendix_B_Dunkelflaute.tex`: Fuel-correlation adjustments.
    * `Appendix_C_Large_Load.tex`: AI/Data Center reliability incidence formulas.

## 🛠️ Compilation
The UEVF Technical Series
This report serves as the mathematical foundation for the broader Unified Energy Valuation Framework:

TP-005: LOLE to Monetized Risk (Policy Governance)

TP-006: Modernizing MISO Deliverability (The "Portfolio-Ready" POI)

TP-008: Accelerated Resource Adequacy Queues (ARQ) (Queue Implementation)

⚖️ Citation
Please utilize the following citation when referencing the MRV formulas, the Dunkelflaute Adjustment, or the Large Load Reliability Penalty:

APA Format

Candler, J., & Uriel. (2025). From Compliance to Value: Monetized Reliability Risk and Prioritizing Interconnection via the EUE × VOLL Standard (Technical Report No. TP-007). Nous Enterprises LLC.
