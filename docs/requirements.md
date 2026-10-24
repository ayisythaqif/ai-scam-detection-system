### Functional Requirements

- **FR1:** The system shall allow users to submit a URL for analysis.
- **FR2:** The system shall extract selected URL features required by the chosen classification method.
- **FR3:** The system shall classify a submitted URL into the risk categories supported by the model.
- **FR4:** The system shall display the classification result and available indicators supporting the result.
- **FR5:** The system shall allow users to submit a phone number for checking against an available scam-report data source.
- **FR6:** The system shall display matching phone-number information and its source when a match is available.
- **FR7:** The system shall display an inconclusive result when available evidence is insufficient to support a reliable assessment.

### Non-Functional Requirements

- **NFR1 – Performance:** The system should return a URL assessment within 3 seconds for at least 95% of requests under a defined test environment and workload.
- **NFR2 – Security:** The system shall validate submitted URLs and shall not automatically navigate to or execute submitted URLs during analysis.
- **NFR3 – Usability:** At least 8 out of 10 representative test users should complete a URL check without assistance during usability testing.
- **NFR4 – Privacy:** The system shall not retain identifiable submitted phone numbers or URLs in application logs unless retention is necessary, disclosed, and appropriately authorized.

*Note: These are proposed targets and must be evaluated during testing.*
