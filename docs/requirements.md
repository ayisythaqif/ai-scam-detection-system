### Requirements and User Stories

#### Functional Requirements

- FR1: The system shall allow users to submit a URL for analysis.
- FR2: The system shall extract selected URL features required by the chosen classification method.
- FR3: The system shall classify a submitted URL into the risk categories supported by the model.
- FR4: The system shall display the classification result and available indicators supporting the result.
- FR5: The system shall allow users to submit a phone number for checking against an available scam-report data source.
- FR6: The system shall display matching phone-number information and its source when a match is available.
- FR7:The system shall display an inconclusive result when available evidence is insufficient to support a reliable assessment.

#### Non-Functional Requirements

- NFR1 – Performance: The system should return a URL assessment within 3 seconds for at least 95% of requests under a defined test environment and workload.
- NFR2 – Security: The system shall validate submitted URLs and shall not automatically navigate to or execute submitted URLs during analysis.
- NFR3 – Usability: At least 8 out of 10 representative test users should complete a URL check without assistance during usability testing.
- NFR4 – Privacy: The system shall not retain identifiable submitted phone numbers or URLs in application logs unless retention is necessary, disclosed, and appropriately authorized.

These are proposed targets and must be evaluated during testing.

#### User Stories

US1: Check a suspicious URL

As an internet user, I want to submit a suspicious URL so that I can understand its potential risk before visiting it.

Acceptance criteria:
1. Given a valid URL, when I submit it, the system displays a supported classification or an inconclusive result.
2. The result page displays the available indicators used to support the assessment.

Linked requirements: FR1, FR2, FR3, FR4, FR7.

US2: Check a suspicious phone number

As an internet user, I want to check a phone number against available scam reports so that I can make a more informed decision before responding.

Acceptance criteria:
1. Given a valid phone number, when a matching record exists, the system displays the available record information and its source.
2. When no matching record exists, the system explains that no record was found and that this does not prove the number is safe.

Linked requirements: FR5, FR6.

US3: Understand uncertain results

As an internet user, I want the system to communicate when evidence is insufficient so that I do not mistake an uncertain assessment for a guarantee of safety.

Acceptance criteria:
1. When the system cannot produce a supported assessment, it displays an inconclusive result.
2. The system advises users to consult trusted sources and avoid sharing sensitive information based solely on the result.

Linked requirements: FR7, NFR4.
