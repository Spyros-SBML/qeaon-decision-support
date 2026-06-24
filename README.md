# q-eAON — Carcinogenicity Decision Support

An interactive implementation of the **evolutionary adverse outcome pathway network (eAON)**
model for carcinogenicity. Define a life-course exposure scenario (one or more stressors, each
weighted by genotoxic and promoter mechanism) and obtain a **life-course malignant-transformation
probability** with Monte-Carlo uncertainty, Shapley mixture apportionment, a static-AOP and TSCE
comparison, and a Safe-and-Sustainable-by-Design substitution comparison.

The whole model runs **client-side in the browser** — no server, no data leaves the user's machine.

## Features
- Exposure-history builder with an **IARC key-characteristics scorer** that derives the genotoxic (g)
  and promoter (p) weights from ticked key characteristics.
- Life-course risk with a 90% credible interval (Monte-Carlo over parameter priors).
- eAON vs static-AOP (toxicological MIE reading) vs TSCE (two-stage clonal-expansion limit).
- Order-independent Shapley apportionment of mixture risk.
- Save/compare alternatives for substitution decisions; JSON report export.

## Provenance
Parameters are anchored to bronchial single-cell data (Yoshida et al. 2020) and lung-cancer
epidemiology (Peto et al. 2000); the model reduces to the Moolgavkar–Venzon–Knudson / Armitage–Doll
multistage models in the appropriate limit (manuscript §6.4).

> **Research prototype.** Illustrative parameters; not a validated regulatory instrument.

## Usage
Open `index.html` in any modern browser, or visit the published GitHub Pages URL.

## Citation
Sarigiannis D.A. & Pienta K.J. *Evolutionary adverse outcome pathway networks: reframing
carcinogenicity as a somatic selection process for next-generation risk assessment.* (in preparation)
