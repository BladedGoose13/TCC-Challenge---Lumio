# SROI-LUMIO

![License](https://img.shields.io/badge/license-CC_BY--NC--ND_4.0-red)
![Status](https://img.shields.io/badge/status-experimental-orange)
![Framework](https://img.shields.io/badge/framework-ESG%20%2F%20SROI-green)

Experimental ESG/SROI decision-support framework integrating causal impact adjustment, uncertainty quantification, and portfolio optimization for internal CSR and sustainability analysis.

---

## Overview

SROI-LUMIO is an experimental multi-criteria framework designed to support:

- ESG portfolio evaluation
- Social impact prioritization
- Internal CSR decision-making
- Monte Carlo uncertainty analysis
- Resource allocation optimization
- Comparative project scoring

The framework extends traditional Social Return on Investment (SROI) methodologies by integrating:

- causal adjustment factors,
- operational friction penalties,
- stakeholder collaboration amplification,
- bounded logarithmic scoring,
- and probabilistic risk analysis.

---

## Technical Document

📄 **Read the full technical whitepaper here:**

[![Open PDF](https://img.shields.io/badge/Open-Know--How.pdf-blue?style=for-the-badge)](./Know-How.pdf)

---

## Core Components

The framework integrates:

- Classical SROI causal adjustments
  - Deadweight
  - Attribution
  - Displacement
  - Drop-off

- ESG multidimensional impact scoring
  - Social
  - Environmental
  - Infrastructure

- Financial return modeling

- Monte Carlo simulation

- Portfolio optimization
  - Knapsack allocation model
  - VaR-based robust allocation

---

## Mathematical Structure

The framework combines social and financial performance into a bounded impact index:

\[
u = [\alpha \cdot PS + \gamma \cdot RM] \cdot FL \cdot FC
\]

followed by a logarithmic bounded transformation:

\[
SROI\text{-}X =
\frac{
2\ln(1+u)
}{
\ln(1+u)+\ln 2
}
\]

which constrains the final score to the interval:

\[
0 \leq SROI\text{-}X < 2
\]

---

## Features

- Multi-criteria ESG scoring
- Portfolio-level prioritization
- Scenario simulation via Monte Carlo
- Sensitivity-aware evaluation
- Internal decision-support orientation
- Transparent causal adjustment structure
- Risk-aware capital allocation

---

## Repository Structure

```plaintext
SROI-LUMIO/
│
├── Descripción.md
├── Know-How.pdf
└── README.md
