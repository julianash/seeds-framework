# SEEDS Sustainability Decision Record (SEEDS-DR) - Example

> **Context:** Example generated for an inpatient physiotherapy evolution system in a hospital setting.  
> **Framework:** SEEDS (Sustainability in Biomedical Software Engineering)  
> **Repository:** [seeds-framework](https://github.com/julianash/seeds-framework)

---

## Record Identification & Context

* **SEEDS-DR ID:** SEEDS-DR-002
* **Decision Context:** Existing digital health system assessment / Workflow adaptation request
* **System or Solution:** Hospital Electronic Health Record (EHR) - Physiotherapy Module
* **Stakeholder Role:** Healthcare Professional (Physiotherapist)

---

## Sustainability Reasoning

* **Sustainability Concern:**  
  Physiotherapists face high cognitive burden and time pressure during intensive care unit (ICU) rounds, and the current text-heavy interface requires excessive manual data entry for routine functional scores (e.g., respiratory parameters and motor scales), increasing the risk of documentation errors and professional burnout.

* **SEEDS Dimension(s):**  
  Individual; Technical

* **Related SEEDS Criterion:**  
  User Experience; Workflow Efficiency; Cognitive Workload; Reliability

* **Expected Sustainability Effect:**  
  First-order individual effect reducing professional cognitive fatigue and documentation time, leading to improved patient safety and better allocation of clinical care time.

---

## Actionable Engineering & Verification

* **Derived Non-Functional Requirement (NFR) / Decision:**  
  The physiotherapy module shall provide structured, pre-populated input templates and quick-scoring widgets for standard respiratory and motor evaluations to minimize redundant free-text entry.

* **Acceptance Criterion:**  
  Physiotherapists shall be able to complete a standard patient daily evolution record in under 3 minutes during ICU rounds; interface usability ratings via standardized questionnaires (e.g., SUS) shall exceed 80 points; data entry errors related to mandatory fields shall decrease by at least 30%.

* **Verification Evidence:**  
  Usability testing sessions with active hospital physiotherapists; task-completion time logs; error-rate tracking reports; user feedback surveys.

---

## Governance & Trade-offs

* **Trade-offs & Dependencies:**  
  Streamlining inputs through rigid templates increases interface efficiency, but must maintain enough flexibility to allow qualitative clinical descriptions for complex, non-standard patient conditions.

* **Decision Status:**  
  Accept with conditions

* **Human Review Notes:**  
  Require review and sign-off from the hospital's lead physiotherapist and clinical informatics committee before back-log prioritization.

---

## Revision History

| Date | Author / Role | Description of Changes | Status |
| :--- | :--- | :--- | :--- |
| 2026-06-15 | SEEDS Research Group / Clinical Analyst | Initial draft derived from hospital physiotherapy workflow assessment | Reviewed |
