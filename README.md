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

## 🧩 Repository Contents

```text
├── examples/
│   ├── Case Analysis Template.html
│   ├── Example - Blurry responsibility after a decision.html
│   ├── Example - Blurry responsibility after a decision.pdf
│   ├── Example - Blurry responsibility after a decision.yaml
│   ├── Example - Praxeological analysis of the bonsai thesis.html
│   ├── Example - Praxeological analysis of the bonsai thesis.pdf
│   ├── Example - Praxeological analysis of the bonsai thesis.yaml
│   ├── Example - Self-application of the model.html
│   ├── Example - Self-application of the model.pdf
│   └── Example - Self-application of the model.yaml
├── model specification/
│   ├── Maturity in Practice - Model Specification.html
│   ├── Maturity in Practice - Model Specification.pdf
│   ├── Maturity in Practice - AH Addon Specification.html
│   └── Maturity in Practice - AH Addon Specification.pdf
├── LICENSE-CC-BY-4.0
├── MIPractice_addon_AH_precision.yaml
├── MIPractice_case_v2.0_full_with_model_reference.yaml
├── MIT-LICENSE
└── README.md
```

**Short description:**

* `MIPractice_case_v2.0_full_with_model_reference.yaml`
  → Single source of truth: normative model (`model_reference`) + case schema (`case`) + agent interface.

* `MIPractice_addon_AH_precision.yaml`
  → Optional **AH Precision addon** (Attack Surface / Hardening): a meta-layer that evaluates the **analysis artefact** for scope drift, language drift, inference risk, and misuse potential (additive only; no score mutation).

* `model specification/`
  → Human- and print-friendly specifications (core model + addon):
  parameters, guardrails, IA-box, dignity framework, bias/intuition/norm-change modules,
  formal notation, case schema, plus the AH addon overlay spec.

* `examples/`
  → Demo cases (YAML + rendered HTML/PDF) and the generic rendering template.

* `MIT-LICENSE`
  → MIT License for code/tooling.

* `LICENSE-CC-BY-4.0`
  → CC BY 4.0 for all model content and documentation.

---

## 🧠 Purpose of This Repository

This repository provides:

* A stable, citable **reference architecture** for praxeological analysis (maturity, asymmetry, responsibility, dignity in practice).
* A transparent, guardrail-based methodology for analysing enactments and structures.
* A **uniform case schema** (`MIPractice_case`) for structured, reversible and dignity-preserving evaluation.
* A machine-interpretable **YAML schema** for:

  * research & teaching
  * supervision, organisational reflection, audits
  * AI / LLM reasoning and governance layers
* A minimal **formal notation** enabling integration with tools, decision-support systems and structured workflows.
* Practical **examples and templates** for:

  * live demos and training
  * leadership / organisational workshops
  * AI-based analysis setups (automatic or interactive / reflective use)
* An optional **AH Precision addon** to strengthen epistemic robustness and reduce misuse risk in high-stakes contexts.

---

## 🧾 The YAML Specification at a Glance

The file **`MIPractice_case_v2.0_full_with_model_reference.yaml`** is the **canonical source** and should be consumed directly (no manual rewrites).

It contains three main blocks:

### 1. `schema_meta` & `agent_interface`

* `schema_meta`

  * canonical name & version
  * status (`stable`)
  * intended-use profiles (self-reflection, professional supervision, organisational audit, training simulation)
  * **red zones** where the model must not be used
    (clinical diagnostics, forensics, individual HR-decisions, child diagnostics, public pillory/ranking)

* `agent_interface`

  * `welcome_message`

    * pre-defined welcome / onboarding text displayed after loading
  * `pre_analysis_questions` (switchboard)

    * reflection mode?
    * D-module usage?
    * analysis depth?
    * output format?
    * discipline_profile?
  * `defaults` (if user does not specify)

    * `reflection_mode: "off"`
    * `d_module_preference: "auto"` (guardrail-aware activation)
    * `analysis_mode: "full"`
    * `output_format: "text"`
    * `discipline_profile: "generic"`
  * `discipline_profiles`

    * domain-specific profiles (sociology, law, psychology, media studies, AI governance, etc.)

This allows consistent integration into AI systems and discipline adaptation without changing axioms.

### 2. `model_reference` – Normative model

Defines the full IA / ACRPD framework:

* parameters A–C–R–P–D and submodule matrix
* guardrails and ethics of use (focus on enactments, D₀ untouchable, system axiom, etc.)
* IA-box (T–J–TB–R) for asymmetry evaluation
* dignity framework (D₀ / D₁ / D₂; D-I/D-B/D-R/D-P)
* scoring rules for:

  * `A(H)` – maturity in practice of an enactment (always a **band**, 0–10)
  * `M(A)` – shared responsibility of an actor (also a **band**, 0–10)
* bias, intuition and norm-change modules
* trajectory patterns (ascending, descending, zigzag, plateau)
* axiomatic core & minimal formal notation (action tuple H, joint notation H ⇒ (A(H), M(A)))
* discipline profiles for field-specific activation of modules and questions

### 3. `case` – Uniform case schema (`MIPractice_case`)

Defines the structured template for any full analysis:

* `meta` & `guardrails`
* `information_basis` & `snapshot`
* `role_mapping` & `frame_vs_variability`
* `acrpd_profile` & `acrpd_submodules_profile`
* `scores_and_ia`
* `ia_protection`
* `trajectory`
* `d_module_optional` (optional, default off)
* `open_questions_and_blind_spots`, `biases_case_level`, `analyst_reflection`, `transmission_check`
* `uniform_report`

---

## 🧩 Optional Addon: AH Precision (Attack Surface / Hardening)

This repository also includes an optional addon:

* **YAML addon contract:** `MIPractice_addon_AH_precision.yaml`
* **Human spec (HTML/PDF):** `model specification/Maturity in Practice - AH Addon Specification.*`

**AH = Attack Surface / Hardening**
A meta-analytic overlay that evaluates the **analysis artefact** (not the person, not the enactments) for:

* scope drift (overgeneralisation)
* moral loading / normative language drift
* trigger ambiguity
* evidence gaps
* reification & instrumentalisation risk

**Integration rule:** additive only (no score mutation; removable without affecting core validity).
**Rendering:** The Case Analysis Template supports an optional AH block that is hidden by default and becomes visible only when addon output is present.

---

## 🤖 Working with AI Agents (LLMs, tools, etc.)

You can either integrate the YAML into your own LLM setup, or use a ready-made **MIPractice / IA agent** in ChatGPT:

> **Start the MIPractice / IA agent in ChatGPT**
> 👉 [Open the “Maturity in Action – A Praxeological Anthropology” agent](https://chat.openai.com/g/g-693460d3def48191ad08647301645a2e-maturity-in-action-a-praxeological-anthropology)
> *(Requires a ChatGPT account with access to custom GPTs; the link may change over time.)*

The YAML is designed to be used **directly** with AI systems.

### 0. Initialisation: loading the YAML

**English:**

```text
Load the YAML file, parse it, and activate the agent_interface.
Then output exactly the text stored in agent_interface.welcome_message.message_text.
Afterwards, use all defaults, guardrails, and pre-analysis logic defined in the YAML.
```

**Deutsch:**

```text
Lade die YAML-Datei vollständig, parse sie und aktiviere den agent_interface.
Gib anschließend exakt den vollständigen Text aus agent_interface.welcome_message.message_text explizit auf deutsch aus.
Danach gelten alle Defaults, Guardrails und pre_analysis-Logiken aus der YAML.
```

### 1. Respect the `agent_interface`

When an AI loads the YAML, it should:

1. Read `agent_interface.pre_analysis_questions.*` to decide whether it should ask about:

   * reflection mode (`on` / `off`)
   * D-module preference (`auto` / `on` / `off`)
   * analysis mode (`ultra_short` / `short` / `full`)
   * output format (`text` / `yaml`)
   * discipline_profile

2. If the user does not specify, use `agent_interface.defaults`.

### 2. Two main usage modes

#### A. Automatic analysis

You provide a thesis or scenario; the AI returns a full `case` block.

#### B. Interactive reflection / supervision

The AI uses the schema as a conversation protocol.

### 3. Rendering as HTML (Case Analysis Template)

For clean, shareable output, you can feed a `case` into the template:

`examples/Case Analysis Template.html`

Typical instruction:

> “Take the MIPractice_case YAML above and insert its content into `Case Analysis Template.html`.
> Replace all placeholders (`{{…}}`) with corresponding case fields.
> Return the completed HTML.”

**If the AH addon is used:**
Provide both YAMLs (core + addon), merge addon output into the case under `addons.ah_precision` (or `uniform_report.addons.ah_precision`), and make the AH block visible in the template.

---

## 🧪 Example Cases

The example cases illustrate different application zones:

1. **Blurry responsibility after a decision**
   → Organisation/team setting; unclear responsibility and communication.

2. **Praxeological analysis of the bonsai thesis**
   → Symbolic/cultural reading; practice + critique style.

3. **Self-application of the model**
   → Meta-case; the model as object of analysis.

Each case is provided as:

* `… .yaml` → structured MIPractice_case instance
* `… .html` → rendered via the template
* `… .pdf` → print- and citation-ready snapshot

---

## 📚 Citation

If you reference the model, please cite both the book and this specification:

**Primary reference:**
T. Zöller (2025). *Maturity in Practice – A Praxeological Anthropology.*

**Technical reference:**
*MIPractice_case v2.0 – Full Schema with Model Reference.* YAML Specification and Case Framework.

**Addon reference (if used):**
*Maturity in Practice – AH Precision Addon Specification* (HTML/PDF) and `MIPractice_addon_AH_precision.yaml`.

---

## 📝 License

This repository uses a **dual-license model**.

### 1. Code (if/where present)

Licensed under the **MIT License** → see `MIT-LICENSE`

### 2. Model content & documentation

Licensed under **CC BY 4.0** → see `LICENSE-CC-BY-4.0`

Applies to:

* `MIPractice_case_v2.0_full_with_model_reference.yaml`
* `MIPractice_addon_AH_precision.yaml`
* all conceptual definitions, guardrails & axioms
* the specifications (HTML/PDF in `model specification/`)
* example analyses and templates in `examples/`

Attribution string:

> “T. Zöller – Maturity in Practice / IA Model (ACRPD / MIPractice_case v2.0)”

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
