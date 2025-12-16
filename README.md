# Maturity in Practice – IA (Inadult Asymmetry) Model Specification

### A praxeological framework for maturity, responsibility, asymmetry & dignity in practice

**Version:** 2.0
**Author:** T. Zöller
**Status:** Public model specification

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.17897159.svg)](https://doi.org/10.5281/zenodo.17897159)

---

## Start here (10 minutes)

If you want to *use* the model (not study it), start with the minimal example:

1. Open: `examples/01_Minimal_Public_Criticism.html`
2. Compare with its structured source: `examples/01_Minimal_Public_Criticism.yaml`
3. To render your own case: copy `examples/00_Case Analysis Template.html` and replace placeholders (`{{…}}`) using a completed MIPractice case.

**Tip (learning-by-doing):** run your first cases with an AI as a trainer: *reflection_mode off* → then *on*.

---

## 🔁 Typical usage workflow (recommended)

MIPractice is designed to be **used iteratively**, ideally with an AI acting as a structured trainer.
You do **not** need to understand the full specification before your first run.

### Step 1 – First structural pass (core model)

**Input:**

* Upload `MIPractice_case_v2.0_full_with_model_reference.yaml`
* Provide a short thesis or scenario (plain text is sufficient)

**Recommended settings:**

* `reflection_mode: off`
* `analysis_mode: full` (or `short` for quick orientation; `ultra_short` for a first glance)
* `output_format: text`

**Goal:**

* Get a clear structural reading (A–C–R–P–D, IA-box, trajectory)
* Identify roles, asymmetries and responsibility patterns

### Step 2 – Guided refinement (learning & clarification)

**Action:**

* Re-run the case with `reflection_mode: on`

**What happens:**

* The AI asks clarifying questions
* Assumptions, blind spots and scope limits become explicit

**Goal:**

* Improve the quality of the case description
* Learn the model by doing, not by reading theory

### Step 3 – Precision & hardening (optional, recommended for publication)

**Additional input:**

* Also upload `MIPractice_addon_AH_precision.yaml`

**Action:**

* Run the AH Precision addon on the completed analysis

**What AH does:**

* Evaluates the **analysis artefact itself**, not the case
* Flags scope drift, moral loading, trigger ambiguity, evidence gaps, and reification/misuse risks

**Goal:**

* Increase epistemic robustness
* Make the analysis safer for external use

### Step 4 – Re-run with a refined thesis (recommended)

**Action:**

* Adjust thesis wording, scene description and scope limitations based on AH output
* Re-run the **core MIPractice analysis** with the refined input

**Result:**

* More precise findings
* Clearer boundaries and better justifications

> **Important:** AH is not a verdict.
> It is a **development and precision layer** that supports re-runs and refinement cycles.

### Step 5 – Rendering & sharing

**Action:**

* Insert the final case output into `examples/00_Case Analysis Template.html`

**Result:**

* Clean, printable HTML / PDF
* Optional AH section automatically visible if addon output exists

---

## 📘 Overview

This repository contains the **official specification** for **Maturity in Practice / IA (inadult asymmetry)** — a praxeological framework for analysing enactments, maturity, responsibility, structural asymmetry and dignity in practice.

The conceptual foundation of this model is presented in the book:

> **T. Zöller (2025): *Maturity in Practice – A Praxeological Anthropology***
> More information: [https://www.amazon.com/dp/B0G6G7V38P](https://www.amazon.com/dp/B0G6G7V38P)

This repository includes:

* the **full technical model specification** (HTML & PDF)
* the **canonical YAML schema** (model + case structure)
* several **worked example cases** (HTML, PDF, YAML)
* a **generic case analysis HTML template**
* the **license files** for code and model content
* an **optional addon** for epistemic precision & misuse resistance (AH Precision)
* an optional **AI agent** that can load and apply the model interactively (see below)

Together, these files form the authoritative public definition of the IA / ACRPD (`MIPractice_case`) model and its optional AH addon.

---

## 🧭 What is this model for?

MIPractice / IA is designed for **structural readings** of human action under real conditions:

* maturity **in action** (not self-image)
* responsibility under uncertainty
* asymmetry checks (power, dependency, opacity)
* dignity in practice (D₀ is untouchable)

It is **not** designed for (red zones):

* clinical diagnosis
* forensics
* individual HR decisions
* child diagnostics
* public ranking / pillorying

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
```

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

You can integrate the YAML into your own LLM setup, or use a ready-made MIPractice/IA agent in ChatGPT:

> Start the MIPractice / IA agent in ChatGPT
> [https://chat.openai.com/g/g-693460d3def48191ad08647301645a2e-maturity-in-action-a-praxeological-anthropology](https://chat.openai.com/g/g-693460d3def48191ad08647301645a2e-maturity-in-action-a-praxeological-anthropology)
> *(Requires a ChatGPT account with access to custom GPTs; the link may change over time.)*

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

This repository uses a **dual-license model** (see `licenses/`).

* `licenses/LICENSE`
  MIT License for code/tooling (scripts, helpers, integration glue).

* `licenses/LICENSE-CC-BY-NC-SA`
  CC BY-NC-SA for model content & documentation (YAML schemas, specifications, examples, templates).

**© 2025 T. Zöller**

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
