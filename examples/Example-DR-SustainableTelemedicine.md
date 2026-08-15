# SEEDS Sustainability Decision Record (SEEDS-DR) - Example

> **Context:** Example generated for a digital health solution intake (Telehealth Platform).  
> **Framework:** SEEDS (Sustainability in Biomedical Software Engineering)  
> **Repository:** [seeds-framework](https://github.com/julianash/seeds-framework)

---

## Record Identification & Context

* **SEEDS-DR ID:** SEEDS-DR-005
* **Decision Context:** Digital health solution intake / Feature design
* **System or Solution:** Telemedicine Platform
* **Stakeholder Role:** Patient / End-User

---

## Sustainability Reasoning

* **Sustainability Concern:**  
  The platform defaults to high-definition video transmission for all consultations. This generates high data traffic and energy demand across the network, which may be unnecessary for clinical tasks that do not require high visual precision, potentially excluding users with limited internet connectivity or mobile data plans.

* **SEEDS Dimension(s):**  
  Environmental (Primary); Social (Secondary); Individual (Secondary)

* **Related SEEDS Criterion:**  
  Energy Efficiency and Resource Use; Data Storage and Transfer; Digital Equity/Access

* **Expected Sustainability Effect:**  
  First-order environmental effect by reducing network energy consumption; secondary social effect by increasing platform accessibility for users with limited bandwidth.

---

## Actionable Engineering & Verification

* **Derived Non-Functional Requirement (NFR) / Decision:**  
  The system shall provide an "Adaptive Quality Mode" that allows the patient/user to select a low-bandwidth/low-energy profile without interrupting the clinical connection.

* **Acceptance Criterion:**  
  The user must be able to switch to low-bandwidth mode in under 3 clicks; the system must demonstrate a minimum 30% reduction in data throughput during the low-bandwidth mode; the clinical connection must remain stable during the mode transition.

* **Verification Evidence:**  
  Network traffic logs per session; user usability testing; accessibility compliance test for the quality-selector component.

---

## Governance & Trade-offs

* **Trade-offs & Dependencies:**  
  Reducing video resolution and data throughput significantly improves environmental sustainability and access equity, but may trade off visual diagnostic clarity, requiring clear clinical guidance on when high-definition is mandatory.

* **Decision Status:**  
  Accept with conditions

* **Human Review Notes:**  
  Must be reviewed by the clinical team to define which types of consultations (e.g., dermatological assessment vs. psychiatry) require HD and which can be conducted in low-bandwidth mode.

---

## Revision History

| Date | Author / Role | Description of Changes | Status |
| :--- | :--- | :--- | :--- |
| 2026-08-15 | SEEDS Research Group / Requirements Engineer | Initial draft for adaptive video quality in telemedicine | Reviewed |
