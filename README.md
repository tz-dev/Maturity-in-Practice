# Maturity in Practice – IA (Inadult Asymmetry) Model Specification

### A praxeological framework for maturity, responsibility, asymmetry & dignity in practice

**Version:** 2.0  
**Author:** T. Zöller  
**Status:** Public model specification  

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.17897159.svg)](https://doi.org/10.5281/zenodo.17897159)

---

## 📘 Overview

This repository contains the **official specification** for **Maturity in Practice / IA (inadult asymmetry)** — a praxeological framework for analysing enactments, maturity, responsibility, structural asymmetry and dignity in practice.

The conceptual foundation of this model is presented in the book:

> **T. Zöller (2025): *Maturity in Practice – A Praxeological Anthropology***  
> (See **Links & Resources** below.)

This repository includes:

- the **full technical model specification** (HTML & PDF)
- the **canonical YAML schema** (model + case structure)
- several **worked example cases** (HTML, PDF, YAML)
- a **generic case analysis HTML template**
- the **license files** for code and model content
- an **optional addon** for epistemic precision & misuse resistance (AH Precision)
- an optional **AI agent** that can load and apply the model interactively (see below)

Together, these files form the authoritative public definition of the IA / ACRPD (`MIPractice_case`) model and its optional AH addon.

---

## 🧭 What is this model for?

MIPractice / IA is a **praxeological analysis framework** for situations where questions of maturity, responsibility and dignity arise **in action**, not in abstract ideals.

It is designed for cases where:
- actions unfold under **real constraints** (time pressure, power asymmetries, role ambiguity),
- responsibility is **distributed or unclear**,
- moral language is present but **insufficient** to understand what is actually happening,
- and outcomes depend on how people act **within structures**, not just on intentions.

The model helps to:
- make **enactments** readable instead of judging persons,
- analyse responsibility **without collapsing into blame or excuse**,
- detect **asymmetries** that distort agency or accountability,
- keep **dignity protected** while still enabling critical analysis,
- and support **learning, repair and improvement**, not verdicts.

Typical application contexts include:
- organisational decision-making and leadership situations,
- professional reflection and supervision,
- analysis of public discourse and moral critique,
- AI-assisted analysis, audits and governance settings,
- research and teaching in praxeological, ethical or social-scientific contexts.

MIPractice / IA is **not** a diagnostic, therapeutic or evaluative scoring system.  
It does not rank people, assign moral worth, or replace professional judgement.

Its purpose is to provide a **structured, reversible and misuse-resistant way** to understand what is happening in complex human action — and what could be done differently.

It is **not** designed for (red zones):
- clinical diagnosis
- forensics
- individual HR decisions
- child diagnostics
- public ranking / pillorying

---

## 🔁 Typical usage workflow (recommended)

MIPractice is designed to be **used iteratively**, ideally with an AI acting as a structured trainer. You do **not** need to understand the full specification before your first run.

### Step 1 – First structural pass (core model)

**Input:**
- Upload `MIPractice_case_v2.0_full_with_model_reference.yaml`
- Provide a short thesis or scenario (plain text is sufficient)

**Recommended settings:**
- `reflection_mode: off`
- `analysis_mode: full` (or `short` for quick orientation; `ultra_short` for a first glance)
- `output_format: text`

**Goal:**
- Get a clear structural reading (A–C–R–P–D, IA-box, trajectory)
- Identify roles, asymmetries and responsibility patterns

### Step 2 – Guided refinement (learning & clarification)

**Action:**
- Re-run the case with `reflection_mode: on`

**What happens:**
- The AI asks clarifying questions
- Assumptions, blind spots and scope limits become explicit

**Goal:**
- Improve the quality of the case description
- Learn the model by doing, not by reading theory

### Step 3 – Precision & hardening (optional, recommended for publication)

**Additional input:**
- Also upload `MIPractice_addon_AH_precision.yaml`

**Action:**
- Run the AH Precision addon on the completed analysis

**What AH does:**
- Evaluates the **analysis artefact itself**, not the case
- Flags scope drift, moral loading, trigger ambiguity, evidence gaps, and reification/misuse risks

**Goal:**
- Increase epistemic robustness
- Make the analysis safer for external use

### Step 4 – Re-run with a refined thesis (recommended)

**Action:**
- Adjust thesis wording, scene description and scope limitations based on AH output
- Re-run the **core MIPractice analysis** with the refined input

**Result:**
- More precise findings
- Clearer boundaries and better justifications

> **Important:** AH is not a verdict.  
> It is a **development and precision layer** that supports re-runs and refinement cycles.

### Step 5 – Rendering & sharing

**Action:**
- Insert the final case output into `examples/00_Case Analysis Template.html`

**Result:**
- Clean, printable HTML / PDF
- Optional AH section automatically visible if addon output exists

---

## 🧩 Repository contents

```text
├── examples/
│   ├── 00_Case Analysis Template.html
│   ├── 01_Minimal_Public_Criticism.html
│   ├── 01_Minimal_Public_Criticism.pdf
│   ├── 01_Minimal_Public_Criticism.yaml
│   ├── 02_Blurry_Responsibility_Org.html
│   ├── 02_Blurry_Responsibility_Org.pdf
│   ├── 02_Blurry_Responsibility_Org.yaml
│   ├── 03_Public_Moral_Critique_with_AH.html
│   ├── 03_Public_Moral_Critique_with_AH.pdf
│   ├── 03_Public_Moral_Critique_with_AH.yaml
│   ├── 04_Meta_Analysis_with_AH.html
│   ├── 04_Meta_Analysis_with_AH.pdf
│   ├── 04_Meta_Analysis_with_AH.yaml
│   ├── 05_Self_Application_of_the_model_on_itself.html
│   ├── 05_Self_Application_of_the_model_on_itself.pdf
│   └── 05_Self_Application_of_the_model_on_itself.yaml
├── licenses/
│   ├── LICENSE
│   └── LICENSE-CC-BY-NC-SA
├── model specification/
│   ├── Maturity in Practice - Model Specification.html
│   ├── Maturity in Practice - Model Specification.pdf
│   ├── Maturity in Practice - AH Addon Specification.html
│   └── Maturity in Practice - AH Addon Specification.pdf
├── MIPractice_case_v2.0_full_with_model_reference.yaml
├── MIPractice_addon_AH_precision.yaml
└── README.md
````

### What each top-level file does (short)

* `MIPractice_case_v2.0_full_with_model_reference.yaml`
  Canonical single source of truth: normative model (`model_reference`) + uniform case schema (`case`) + `agent_interface`.

* `MIPractice_addon_AH_precision.yaml`
  Optional **AH Precision addon** (Attack Surface / Hardening): evaluates the **analysis artefact** for scope drift, language drift, inference risk, and misuse potential.
  **Additive only** (no score mutation; removable).

---

## ✅ Examples (from easiest to most complex)

All examples are available as **YAML + HTML + PDF**.

1. **01 – Minimal Public Criticism**
   `examples/01_Minimal_Public_Criticism.*`
   Minimal entry case: single scene, clear trigger, two trajectories.

2. **02 – Blurry Responsibility (Organisation)**
   `examples/02_Blurry_Responsibility_Org.*`
   Typical organisational case: decision taken, responsibility & communication unclear.

3. **03 – Public Moral Critique (with AH)**
   `examples/03_Public_Moral_Critique_with_AH.*`
   Public discourse case; AH addon enabled to show precision/misuse risks.

4. **04 – Meta Analysis (with AH)**
   `examples/04_Meta_Analysis_with_AH.*`
   Analysis-of-analysis case; AH addon is central.

5. **05 – Self-Application of the model on itself**
   `examples/05_Self_Application_of_the_model_on_itself.*`
   Advanced meta-case: the model reads its own design.

---

## 🧩 Optional addon: AH Precision (Attack Surface / Hardening)

This repository includes an optional addon:

* **YAML addon contract:** `MIPractice_addon_AH_precision.yaml`
* **Human spec (HTML/PDF):** `model specification/Maturity in Practice - AH Addon Specification.*`

**AH = Attack Surface / Hardening**
A meta-analytic overlay that evaluates the **analysis artefact** (not the person, not the enactments) for:

* scope drift (overgeneralisation)
* moral loading / normative language drift
* trigger ambiguity
* evidence gaps
* reification & instrumentalisation risk

**When to use AH (recommended):**

* you publish or share analyses externally
* you run analyses in audits / governance settings
* you automate analysis generation (LLMs)
* you expect adversarial readings / misuse risk

**When to skip AH (usually fine):**

* private reflection / early drafts
* simple training runs
* internal supervision where reversibility is guaranteed

AH is intentionally designed to support **re-runs and refinement cycles**, not to freeze or finalise interpretations.

**Integration rule:** additive only (no score mutation; removable without affecting core validity).
**Rendering:** the Case Analysis Template contains an AH block that is hidden by default and becomes visible only when addon output is present.

---

## 📄 Model specifications (human-readable)

* Core model specification:
  `model specification/Maturity in Practice - Model Specification.html`
  `model specification/Maturity in Practice - Model Specification.pdf`

* AH addon specification:
  `model specification/Maturity in Practice - AH Addon Specification.html`
  `model specification/Maturity in Practice - AH Addon Specification.pdf`

---

## 🤖 Using AI as a trainer (recommended)

You can integrate the YAML into your own LLM setup, or use a ready-made MIPractice/IA agent in ChatGPT (see **Links & Resources** above).

### Minimal loader instruction (English)

```text
Load MIPractice_case_v2.0_full_with_model_reference.yaml, parse it, and activate agent_interface.
Use defaults unless I specify otherwise.
Then guide me through a first case with reflection_mode: off.
```

### Minimal loader instruction (Deutsch)

```text
Lade MIPractice_case_v2.0_full_with_model_reference.yaml vollständig, parse sie und aktiviere agent_interface.
Nutze Defaults, sofern ich nichts anderes angebe.
Führe mich dann durch einen ersten Fall mit reflection_mode: off.
```

### Rendering to HTML (template)

Template file:

* `examples/00_Case Analysis Template.html`

Typical instruction to an AI:

```text
Take the completed MIPractice_case YAML output and insert its content into examples/00_Case Analysis Template.html.
Replace all placeholders {{…}} with the corresponding case fields.
Return the completed HTML.
If AH addon output exists, make the AH section visible and fill the AH fields.
```

---

## 🔗 Links & Resources

*Maturity in Practice* is situated within a broader **praxeological ecosystem** that connects anthropological theory, formal operator models, applied analyses, and executable specifications.  

The resources below are organized by **structural role** within that ecosystem.  

| Category        | Resource                                                                                                                                                                                                                     | Description                                                                                     |
| --------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| Model website   | https://pms-theory.netlify.app                                                                                                                                                                                               | Canonical PMS theory reference                                                                  |
| Book websites   | https://maturity-in-practice.netlify.app                                                                                                                                                                                     | *Maturity in Practice* — English edition (praxeological anthropology)                           |
|                 | https://reife-im-vollzug.netlify.app                                                                                                                                                                                         | *Reife im Vollzug* — Deutsche Ausgabe                                                           |
|                 | https://pms-stack.netlify.app                                                                                                                                                                                               | PMS-STACK reference architecture                                                                |
| Amazon          | https://www.amazon.com/dp/B0G4XBKNNR                                                                                                                                                                                         | *Maturity in Practice: A Praxeological Anthropology* — English edition                          |
|                 | https://www.amazon.de/dp/B0G4SPBDQD                                                                                                                                                                                          | *Reife im Vollzug: Eine praxeologische Anthropologie* — Deutsche Ausgabe                        |
|                 | https://www.amazon.com/dp/B0G6G7V38P                                                                                                                                                                                         | *PMS-STACK — A Praxeological Operating System Architecture*                                     |
| GitHub (papers) | https://github.com/tz-dev/Praxeological-Meta-Structure-Theory                                                                                                                                                               | Canonical PMS grammar, theory & YAML definitions                                                |
|                 | https://github.com/tz-dev/Maturity-in-Practice                                                                                                                                                                               | Book sources & applied praxeological anthropology                                               |
|                 | https://github.com/tz-dev/PMS-QC                                                                                                                                                                                             | PMS-QC — Praxeological Meta-Structure for Quantum Computing                                     |
|                 | https://github.com/tz-dev/PMS-LOGIC                                                                                                                                                                                          | PMS-LOGIC — Structural Responsibility, Logical Limits, and Post-Moral Effects                  |
|                 | https://github.com/tz-dev/PMS-ANTICIPATION                                                                                                                                                                                    | PMS-ANTICIPATION — Structural Conditions, Risks, and Viability of Anticipatory Praxis           |
|                 | https://github.com/tz-dev/PMS-CRITIQUE                                                                                                                                                                                       | PMS-CRITIQUE — From Irritation to Correction: A Praxeological Grammar of Critique               |
|                 | https://github.com/tz-dev/PMS-EDEN                                                                                                                                                                                           | PMS-EDEN — Structural Drift from Praxis to Comparison and Reciprocity Loss                      |
|                 | https://github.com/tz-dev/PMS-SEX                                                                                                                                                                                            | PMS-SEX — From Impulse to Self-Binding: A Praxeological Grammar of Sexuality                    |
|                 | https://github.com/tz-dev/PMS-CONFLICT                                                                                                                                                                                       | PMS-CONFLICT — Conflict as Stabilized Incompatibility: Cost, Binding, and Tragic Non-Integration |
| Custom GPTs     | https://chatgpt.com/g/g-69358a2a4980819183da6a97893389cf-pms-model-assistant                                                                                                                                                  | Interactive PMS.yaml exploration & validation                                                   |
|                 | https://chat.openai.com/g/g-693460d3def48191ad08647301645a2e-maturity-in-action-a-praxeological-anthropology                                                                                                                 | Applied praxeological anthropology assistant                                                    |

---

## 📚 Citation

If you reference the model, please cite both the book and this specification:

**Primary reference:**
T. Zöller (2025). *Maturity in Practice – A Praxeological Anthropology.*

**Technical reference:**
*MIPractice_case v2.0 – Full Schema with Model Reference.* YAML Specification and Case Framework.

**Addon reference (if used):**
*Maturity in Practice – AH Precision Addon Specification* and `MIPractice_addon_AH_precision.yaml`.

---

## 📝 Licenses

This repository uses a **dual-license model**.

* `MIT-LICENSE`
  MIT License for code and tooling (scripts, helpers, integration glue).

* `LICENSE-CC-BY-4.0`
  Creative Commons Attribution 4.0 International for all model content and documentation
  (YAML schemas, specifications, examples, templates).

> “T. Zöller – Maturity in Practice / IA Model (ACRPD / MIPractice_case v2.0)”

---

## 🤝 Contributing

Contributions (issues, fixes, example tooling, integrations) are welcome.

Before submitting changes, please open an issue to:

* clarify scope
* ensure compatibility with the YAML schema
* avoid breaking changes to `model_reference` and `case` structure

---

## 🧭 Versioning

This project follows semantic versioning for the YAML schema and model:

* Minor versions keep structural compatibility within `model_reference` / `case`
* Major versions may introduce breaking changes
* Documentation and examples reference the YAML version they correspond to

Current schema version:
**`MIPractice_case_v2.0_full_with_model_reference`**
