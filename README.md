# Maturity in Practice – IA (Inadult Asymmetry) Model Specification  
### A praxeological framework for maturity, responsibility, asymmetry & dignity in practice

**Version:** 2.0  
**Author:** T. Zöller  
**Status:** Public model specification  

---

## 📘 Overview

This repository contains the **official specification** for  
**Maturity in Practice / IA (inadult asymmetry)** — a praxeological framework for analysing
enactments, maturity, responsibility, structural asymmetry and dignity in practice.

The conceptual foundation of this model is presented in the book:

> **T. Zöller (2025): _Maturity in Practice – A Praxeological Anthropology_**  
> More information: https://www.maturity-in-practice.com/

This repository includes:

- the **full technical model specification** (HTML & PDF)  
- the **canonical YAML schema** (model + case structure)  
- several **worked example cases** (HTML, PDF, YAML)  
- a **generic case analysis HTML template**  
- the **license files** for code and model content

Together, these files form the authoritative public definition of the IA / ACRPD model.

---

## 🧩 Repository Contents

```text
├── MIPractice_case_v2.0_full_with_model_reference.yaml                 # Canonical YAML model + case schema
├── model specificaton/
│   ├── Maturity in Practice - Model Specification.html                 # Human-readable spec
│   └── Maturity in Practice - Model Specification.pdf                  # Print- & citation-ready spec
├── examples/
│   ├── Case Analysis Template.html                                     # Generic MIPractice_case HTML template
│   ├── Example - Blurry responsibility after a decision.html           # Rendered demo case (ACRPD / IA)
│   ├── Example - Blurry responsibility after a decision.pdf            # Print-ready version
│   ├── Example - Blurry responsibility after a decision.yaml           # YAML demo case (MIPractice_case)
│   ├── Example - Praxeological analysis of the bonsai thesis.html      # Rendered demo case (symbolic/cultural)
│   ├── Example - Praxeological analysis of the bonsai thesis.pdf       # Print-ready version
│   ├── Example - Praxeological analysis of the bonsai thesis.yaml      # YAML demo case (MIPractice_case)
│   ├── Example - Self-application of the model.html                    # Rendered meta-case (model analyses itself)
│   ├── Example - Self-application of the model.pdf                     # Print-ready version
│   └── Example - Self-application of the model.yaml                    # YAML demo case (MIPractice_case)
└── licenses/
    ├── LICENSE                                                         # MIT (for code/tools)
    └── LICENSE-CC-BY-NC-SA                                             # CC BY-NC-SA (for model content)
````

**Short description:**

* `MIPractice_case_v2.0_full_with_model_reference.yaml`
  → Single source of truth: normative model (`model_reference`) + case schema (`case`) + agent interface.

* `model specificaton/`
  → Human- and print-friendly model specification:
  parameters, guardrails, IA-box, dignity framework, bias/intuition/norm-change modules,
  formal notation, and case schema.

* `examples/`

  * `Case Analysis Template.html`
    – Empty MIPractice_case HTML template, used to render any completed case analysis
    (e.g. from YAML or direct AI output) into a clean, printable layout.

  * `Example - Blurry responsibility after a decision.*`
    – Short organisational case: a decision has been taken, but responsibility and
    communication remain blurry.
    – Shows how A/M-bands, IA-box and structural responsibility work in a typical team/organisation setting.

  * `Example - Praxeological analysis of the bonsai thesis.*`
    – Symbolic / cultural case: a philosophical “bonsai thesis” reads an aesthetic practice
    as symptom of problematic self-/other-treatment.
    – Demonstrates how the model can be used on cultural practices and critique styles.

  * `Example - Self-application of the model.*`
    – Meta-case: the MIPractice_case model is applied to itself as an object of analysis.
    – Shows how the axioms, guardrails, IA-box and D-module behave when the model
    reads its own design.

  Each example case is provided as:

  * `… .yaml` → structured MIPractice_case instance
  * `… .html` → rendered via the case analysis template
  * `… .pdf` → print- and citation-ready snapshot

* `licenses/`

  * `LICENSE` – MIT License for code/tooling.
  * `LICENSE-CC-BY-NC-SA` – CC BY-NC-SA 4.0 for all model content and documentation.

---

## 🧠 Purpose of This Repository

This repository provides:

* A stable, citable **reference architecture** for praxeological analysis
  (maturity, asymmetry, responsibility, dignity in practice).

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

---

## 🧾 The YAML Specification at a Glance

The file
**`MIPractice_case_v2.0_full_with_model_reference.yaml`**
is the **canonical source** and should be consumed directly (no manual rewrites).

It contains three main blocks:

### 1. `schema_meta` & `agent_interface`

* `schema_meta`

  * canonical name & version
  * status (`stable`)
  * intended-use profiles (self-reflection, professional supervision, organisational audit, training simulation)
  * **red zones** where the model must not be used
    (clinical diagnostics, forensics, individual HR-decisions, child diagnostics, public pillory/ranking)

* `agent_interface`

  * `pre_analysis_questions` – switchboard for AI behaviour:

    * ask about reflection mode?
    * ask about D-module?
    * ask about analysis depth?
    * ask about output format?
  * `defaults` – what an AI should do **if the user does not specify**:

    * `reflection_mode: "off"`
    * `d_module_preference: "auto"` (guardrail-aware activation)
    * `analysis_mode: "full"`
    * `output_format: "text"`

This allows you to plug the model into AI systems in a consistent way.

### 2. `model_reference` – Normative model

Defines the full IA / ACRPD framework:

* parameters A–C–R–P–D and the **submodule matrix**
* guardrails and ethics of use (focus on enactments, D₀ untouchable, system axiom, etc.)
* IA-box (T–J–TB–R) for asymmetry evaluation
* dignity framework (D₀ / D₁ / D₂; D-I/D-B/D-R/D-P)
* scoring rules for:

  * `A(H)` – maturity in practice of an enactment (always a **band**, 0–10)
  * `M(A)` – shared responsibility of an actor (also a **band**, 0–10)
* bias, intuition and norm-change modules
* trajectory patterns (ascending, descending, zigzag, plateau)
* axiomatic core & minimal formal notation (action tuple H, joint notation H ⇒ (A(H), M(A)))

### 3. `case` – Uniform case schema (`MIPractice_case`)

Defines the structured template for any full analysis:

* `meta` & `guardrails`

  * case ID, title, date, analysts, confidentiality level
  * application zone (green / yellow / red_forbidden)
  * interaction profile for AI use (reflection mode, D-module preference, output format)
  * guardrails: focus on structures, minimal adulthood, dignity protection, tragedy clause, language hygiene

* `information_basis` & `snapshot`

  * primary / secondary material
  * assumptions & inferences
  * coverage & reliability estimates, known gaps, bias risks
  * short case description, central actors/roles, guiding question

* `role_mapping` & `frame_vs_variability`

  * who/what is the object of observation (role, type, description)
  * other relevant roles and typical asymmetries
  * frame elements (laws, hard constraints) vs. variable elements (process, communication)
  * zones where high M would be unfair; misuse of “system” as excuse

* `acrpd_profile` & `acrpd_submodules_profile`

  * core A–C–R–P–D reading
  * optional fine-grained submodule profile for complex cases

* `scores_and_ia`

  * A-band and M-band (bands + justification bullets)
  * IA-box (T/J/TB/R with true/false/unclear + justification)
  * IA summary label (functional_asymmetry / IA_risk / inadulte_asymmetry)

* `ia_protection`

  * documentation of transparency, time-bound measures, reversibility, participation level

* `trajectory`

  * key time points (t0/t1/t2 …) with A- and M-bands
  * narrative course description and responsibility–viability range

* `d_module_optional` (optional, default off)

  * activation reason & guardrail checklist
  * communication space (self, professional_confidential, aggregated_public, structural_public)
  * quick D-grid (0–3) and short D-profile (D1/D2 via D-I/D-B/D-R/D-P)
  * red-zone flags and D-guardrails

* `open_questions_and_blind_spots`, `biases_case_level`, `analyst_reflection`, `transmission_check`

  * explicit documentation of remaining uncertainties, distortions and analyst self-implication
  * check whether the analysis is ready for structural decisions or should remain reflective-only

* `uniform_report`

  * standardised, human-readable summary (overview, key findings, maturity & IA summary, D summary, trajectory, open questions, conclusion)

---

## 🤖 Working with AI Agents (LLMs, tools, etc.)

The YAML is designed to be used **directly** with AI systems.

### 1. Respect the `agent_interface`

When an AI loads the YAML, it should:

1. Read `agent_interface.pre_analysis_questions.*` to see whether it **should ask** about:

   * reflection mode (`on` / `off`)
   * D-module preference (`auto` / `on` / `off`)
   * analysis mode (`ultra_short` / `short` / `full`)
   * output format (`text` / `yaml`)

2. If the user **does not specify**, use `agent_interface.defaults`:

   * `reflection_mode: "off"`
   * `d_module_preference: "auto"`
   * `analysis_mode: "full"`
   * `output_format: "text"`

You can also override this explicitly, e.g.:

> “No reflection mode, activate D if it makes sense, full analysis, YAML output.”

### 2. Two main usage modes

Once the YAML is loaded, there are two typical patterns:

#### **A. Automatic analysis**

You provide a thesis or scenario; the AI returns a full `case` block:

> “Analyse the following scenario using the MIPractice_case template (automatic mode, full analysis, YAML output):
> *‘A decision has been taken in a team, but responsibility and communication are blurry…’*”

The AI then fills:

* `case.meta`, `guardrails`, `information_basis`
* `acrpd_profile`, `scores_and_ia`, `trajectory`, etc.
* optional `d_module_optional` (if `d_module_preference` and guardrails allow it)

#### **B. Interactive reflection / supervision**

The AI uses the schema as a conversation protocol, e.g.:

> “Use the MIPractice_case in interactive mode.
> Ask me step by step about snapshot, information_basis, A–C–R–P–D, A/M-bands, IA-box and trajectory.”

This is useful for self-reflection, supervision, workshops or training.

### 3. Rendering as HTML (Case Analysis Template)

For clean, shareable output, you can feed a `case` into the HTML template:

`examples/Case Analysis Template.html`

A typical instruction to an AI might be:

> “Take the MIPractice_case YAML above and insert its content into `Case Analysis Template.html`.
> Replace all placeholders (`{{…}}`) with the corresponding case fields
> (snapshot, ACRPD, IA-Box, A/M-bands, key findings, conclusion, trajectory).
> Return the completed HTML.”

The examples in `examples/` show how that looks in practice:

* **Blurry responsibility after a decision** – organisational case
* **Praxeological analysis of the bonsai thesis** – symbolic / cultural case
* **Self-application of the model** – meta-case

---

## 🧪 Example Cases

The three example cases illustrate different application zones of the model:

1. **Blurry responsibility after a decision**
   → Organisation / team setting; unclear responsibility and communication; IA_risk in how the decision is carried and communicated.

2. **Praxeological analysis of the bonsai thesis**
   → Philosophical / cultural reading; the bonsai practice as metaphor for self-/other-treatment; joint reading of the criticised practice and the style of critique.

3. **Self-application of the model**
   → The model as object of analysis; shows how IA-box, A/M-bands, D-module and bias/norm-change behave when the framework reflects on itself.

Each case is fully structured (`… .yaml`) and rendered (`… .html` / `… .pdf`), and can be used as:

* templates for new analyses,
* integration tests for tooling,
* teaching material in seminars or workshops.

---

## 📚 Citation

If you reference the model, please cite both the book and this specification:

**Primary reference:**
T. Zöller (2025). *Maturity in Practice – A Praxeological Anthropology.*

**Technical reference:**
*MIPractice_case v2.0 – Full Schema with Model Reference.*
YAML Specification and Case Framework.

---

## 📝 License

This repository uses a **dual-license model**.

### 1. Code (if/where present)

Licensed under the **MIT License**
→ see `licenses/LICENSE`

This applies to:

* scripts, tools, or future code in this repository
* integration helpers you might add (as long as they are code only)

### 2. Model content & documentation

Licensed under
**Creative Commons Attribution–NonCommercial–ShareAlike 4.0 (CC BY-NC-SA 4.0)**
→ see `licenses/LICENSE-CC-BY-NC-SA`

This applies to:

* `MIPractice_case_v2.0_full_with_model_reference.yaml`
* all conceptual definitions, guardrails & axioms
* the Model Specification (HTML & PDF in `model specificaton/`)
* example analyses and templates in `examples/`
* any other non-code documentation in this repository

**© 2025 T. Zöller**

**Summary:**

* ✔ Free for **non-commercial**, educational and research use
* ✔ Derivatives allowed **with attribution** and **same license** (ShareAlike)
* ✖ No commercial use without **explicit written permission**
* ✖ No proprietary forks of the model content

This protects the theoretical model while allowing open collaboration and
MIT-licensed tooling around it.

---

## 🤝 Contributing

Contributions (issues, fixes, example tooling, integrations) are welcome —
as long as they respect the **CC BY-NC-SA** restrictions for model content
(e.g., no commercial forks, no altered model sold as proprietary framework).

Before submitting changes, please open an issue to:

* clarify scope
* ensure compatibility with the YAML schema
* avoid breaking changes to `model_reference` and `case` structure

---

## 🧭 Versioning

This project follows semantic versioning for the YAML schema and model:

* **Minor versions** keep structural compatibility within `model_reference` / `case`
* **Major versions** may introduce breaking changes
* Documentation and examples always reference the YAML version they correspond to

Current schema version:
**`MIPractice_case_v2.0_full_with_model_reference`**

---

## 📬 Contact

For permissions, academic collaboration or commercial licensing:

* **Email:** [info@maturity-in-practice.com](mailto:info@maturity-in-practice.com)
* **Website:** [https://www.maturity-in-practice.com](https://www.maturity-in-practice.com)

