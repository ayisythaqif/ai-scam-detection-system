### US1: Check a Suspicious URL

**User Story:**

As an internet user, I want to submit a suspicious URL so that I can understand its potential risk before visiting it.

**Acceptance Criteria:**

1. Given a valid URL, when I submit it, the system displays a supported classification or an inconclusive result.
2. The result page displays the available indicators used to support the assessment.

**Linked Requirements:** FR1, FR2, FR3, FR4, FR7.

### US2: Check a Suspicious Phone Number

**User Story:**

As an internet user, I want to check a phone number against available scam reports so that I can make a more informed decision before responding.

**Acceptance Criteria:**

1. Given a valid phone number, when a matching record exists, the system displays the available record information and its source.
2. When no matching record exists, the system explains that no record was found and that this does not prove the number is safe.

**Linked Requirements:** FR5, FR6.

### US3: Understand Uncertain Results

**User Story:**

As an internet user, I want the system to communicate when evidence is insufficient so that I do not mistake an uncertain assessment for a guarantee of safety.

**Acceptance Criteria:**

1. When the system cannot produce a supported assessment, it displays an inconclusive result.
2. The system advises users to consult trusted sources and avoid sharing sensitive information based solely on the result.

**Linked Requirements:** FR7, NFR4.
