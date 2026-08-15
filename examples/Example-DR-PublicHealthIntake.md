# SEEDS Sustainability Decision Record (SEEDS-DR) - Example

> **Context:** Example generated for a digital health solution intake (Adoption of a regional Electronic Health Record platform for public health networks).  
> **Framework:** SEEDS (Sustainability in Biomedical Software Engineering)  
> **Repository:** [seeds-framework](https://github.com/julianash/seeds-framework)

---

## Record Identification & Context

* **SEEDS-DR ID:** SEEDS-DR-006
* **Decision Context:** Digital health solution intake / Public health procurement
* **System or Solution:** Regional Public Electronic Health Record (EHR) Platform
* **Stakeholder Role:** Public Health Manager / Institutional Administrator

---

## Sustainability Reasoning

* **Sustainability Concern:**  
  The proposed centralized cloud architecture for the regional public health network relies on resource-heavy, always-on commercial cloud instances with redundant data replication across distant regions, raising long-term public maintenance costs, vendor lock-in risks, and unnecessary carbon footprints from cloud energy consumption.

* **SEEDS Dimension(s):**  
  Economic (Primary); Technical (Secondary); Environmental (Tertiary)

* **Related SEEDS Criterion:**  
  Risk Management and Financial Sustainability; Architectural Interoperability; Energy Efficiency and Resource Use

* **Expected Sustainability Effect:**  
  First-order economic effect ensuring long-term public budget predictability; second-order technical effect preventing vendor lock-in; third-order environmental effect by reducing the aggregate carbon footprint and energy waste of public data centers.

---

## Actionable Engineering & Verification

* **Derived Non-Functional Requirement (NFR) / Decision:**  
  The solution provider shall provision a hybrid or optimized cloud deployment model that supports dynamic resource scaling, off-peak workload shifting, and compliance with green-hosting data center certifications.

* **Acceptance Criterion:**  
  The vendor must present architecture documentation proving resource-efficient scaling; infrastructure cost projections must remain within the municipal health IT budget over a 5-year horizon; data center hosting partners must provide verified energy-efficiency or renewable energy compliance metrics.

* **Verification Evidence:**  
  Vendor architectural proposals; 5-year total cost of ownership (TCO) financial audit; cloud provider green-energy certifications; resource utilization and carbon-emission telemetry reports.

---

## Governance & Trade-offs

* **Trade-offs & Dependencies:**  
  Enforcing optimized resource allocation and green-hosting requirements may increase the initial administrative complexity of the procurement and contract-negotiation process, but it yields substantial long-term economic savings and reduces environmental impact.

* **Decision Status:**  
  Accept with conditions

* **Human Review Notes:**  
  Requires formal alignment between the municipal health procurement department, the technical IT advisory board, and the regional sustainability committee before signing the software adoption agreement.

---

## Revision History

| Date | Author / Role | Description of Changes | Status |
| :--- | :--- | :--- | :--- |
| 2026-08-15 | SEEDS Research Group / Public Health Evaluator | Initial draft for regional EHR solution intake and evaluation | Reviewed |
