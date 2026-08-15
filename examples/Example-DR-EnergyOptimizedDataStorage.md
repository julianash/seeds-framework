# SEEDS Sustainability Decision Record (SEEDS-DR) - Example

> **Context:** Example generated for a Software Adaptation Request focusing on environmental efficiency in large-scale biomedical data storage.  
> **Framework:** SEEDS (Sustainability in Biomedical Software Engineering)  
> **Repository:** [seeds-framework](https://github.com/julianash/seeds-framework)

---

## Record Identification & Context

* **SEEDS-DR ID:** SEEDS-DR-004
* **Decision Context:** Software adaptation request / Architectural optimization
* **System or Solution:** Large-scale Genomics Data Repository
* **Stakeholder Role:** Lead Developer / DevOps Engineer

---

## Sustainability Reasoning

* **Sustainability Concern:**  
  The current storage policy keeps all longitudinal patient imaging and genomic raw data in high-performance hot storage, resulting in excessive energy consumption for data that is rarely accessed after the initial clinical processing.

* **SEEDS Dimension(s):**  
  Environmental (Primary); Economic (Secondary)

* **Related SEEDS Criterion:**  
  Energy Efficiency and Resource Use; Data Storage and Transfer; Governance and Environmental Monitoring

* **Expected Sustainability Effect:**  
  First-order environmental effect by reducing power consumption of data centers; secondary economic effect by lowering high-performance storage infrastructure costs.

---

## Actionable Engineering & Verification

* **Derived Non-Functional Requirement (NFR) / Decision:**  
  The system shall implement an automated lifecycle policy to migrate raw genomic data to cold storage (object storage) after 6 months of inactivity, while maintaining metadata in hot storage.

* **Acceptance Criterion:**  
  The storage energy footprint (kWh/TB) shall be reduced by at least 20% within the first 12 months; data recovery time from cold storage must not exceed 24 hours (SLA threshold).

* **Verification Evidence:**  
  Energy consumption monitoring logs; storage cost analysis reports; data access frequency metrics; performance tests for cold storage retrieval.

---

## Governance & Trade-offs

* **Trade-offs & Dependencies:**  
  While migrating data to cold storage significantly reduces energy consumption and infrastructure costs (economic gain), it introduces retrieval latency, increasing the operational effort if retrospective research requires rapid access to archived raw data.

* **Decision Status:**  
  Accept with conditions

* **Human Review Notes:**  
  Requires approval from the Clinical Research Committee to confirm that the 6-month inactivity window for raw genomic data aligns with clinical and research availability needs.

---

## Revision History

| Date | Author / Role | Description of Changes | Status |
| :--- | :--- | :--- | :--- |
| 2026-08-15 | SEEDS Research Group / DevOps Team | Initial draft for energy-optimized storage migration | Reviewed |
