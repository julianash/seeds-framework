# SEEDS Sustainability Decision Record (SEEDS-DR) - Example

> **Context:** Example generated for a software adaptation request (Migration of legacy electronic health records to a modular microservice architecture).  
> **Framework:** SEEDS (Sustainability in Biomedical Software Engineering)  
> **Repository:** [seeds-framework](https://github.com/julianash/seeds-framework)

---

## Record Identification & Context

* **SEEDS-DR ID:** SEEDS-DR-003
* **Decision Context:** Software adaptation request / Architectural evolution
* **System or Solution:** Legacy Hospital Information System (HIS)
* **Stakeholder Role:** Lead Software Architect / IT Technical Team

---

## Sustainability Reasoning

* **Sustainability Concern:**  
  The monolithic architecture of the legacy HIS suffers from severe technical debt, making incremental updates slow, risky, and costly, while hindering interoperability with external digital health platforms.

* **SEEDS Dimension(s):**  
  Technical; Economic

* **Related SEEDS Criterion:**  
  Maintainability; Interoperability; Technical Debt; Long-term Cost Predictability

* **Expected Sustainability Effect:**  
  Second-order technical and economic effects improving system maintainability, reducing long-term maintenance costs, and enabling safer modular extensions.

---

## Actionable Engineering & Verification

* **Derived Non-Functional Requirement (NFR) / Decision:**  
  The core patient data management modules shall be refactored into decoupled microservices adhering to standard healthcare interoperability protocols (e.g., FHIR).

* **Acceptance Criterion:**  
  The refactored modules must pass automated regression test suites with $\ge 85\%$ code coverage; API response times must remain within baseline thresholds; architectural modularity metrics (e.g., coupling and cohesion) must satisfy defined thresholds.

* **Verification Evidence:**  
  Static code analysis reports; automated CI/CD test results; architecture compliance audits; interoperability conformance test logs.

---

## Governance & Trade-offs

* **Trade-offs & Dependencies:**  
  Migrating to a microservice architecture improves long-term maintainability and technical sustainability, but significantly increases short-term economic costs, operational complexity, and the need for specialized team training.

* **Decision Status:**  
  Accept with conditions

* **Human Review Notes:**  
  Requires financial approval from hospital management and a phased rollout plan to mitigate service disruption risks during the transition period.

---

## Revision History

| Date | Author / Role | Description of Changes | Status |
| :--- | :--- | :--- | :--- |
| 2026-06-20 | SEEDS Research Group / IT Architecture Team | Initial draft for legacy system architectural refactoring | Reviewed |
