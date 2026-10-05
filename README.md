# Networkwalks B083 — Week 4
## Mediroza General Hospital Web Penetration Testing

> Authorized black-box web application penetration-testing assessment completed within the Networkwalks B083 educational environment.

**Target:** `https://medirozahospital.com`  
**Assessment Type:** Black-box web penetration test  
**Duration:** 5 days  
**Environment:** Authorized training lab

---

## Project Overview

This public repository presents the portfolio-safe documentation of the Week 4 Mediroza General Hospital web penetration-testing exercise.

The assessment followed a progressive black-box workflow covering reconnaissance, web enumeration, authentication and input-handling testing, restricted-area access, protected-document assessment, metadata/content analysis, and investigation of an exposed legacy resource.

Sensitive raw artifacts from the exercise are intentionally **not published** in this public repository.

---

## Scope & Rules of Engagement

### In Scope
- Mediroza web application
- Authentication functionality
- Web-accessible directories and resources
- Patient-report functionality
- Publicly accessible resources discovered during testing

### Out of Scope
- Social engineering
- Denial-of-service testing
- Destructive testing
- Systems outside the authorized target

All activities were performed only within the authorized educational environment.

---

## Assessment Objectives

### M1 — Initial Access
Identify and validate a web-application weakness that could provide unauthorized access to restricted functionality.

### M2 — Data Extraction
Assess the protection applied to three retrieved patient-report PDFs and demonstrate whether their passwords could be recovered in the authorized lab environment.

### M3 — Critical Data Exposure
Investigate information obtained during testing and determine whether additional sensitive information was exposed through publicly accessible resources.

### M4 — Final Reporting
Produce the required professional penetration-testing report documenting findings, impact, severity, and remediation.

**M4 report:** intentionally not included in this public portfolio repository.

---

## Methodology

The assessment followed a progressive workflow:

1. Reconnaissance
2. Web technology identification
3. Directory and resource enumeration
4. Authentication testing
5. Username and input-handling testing
6. SQL injection validation
7. Restricted-area access validation
8. Protected-document assessment
9. Password/hash recovery testing
10. PDF decryption validation
11. PDF metadata and content analysis
12. Legacy resource investigation
13. Exposed-backup validation
14. Sensitive-data impact assessment
15. Evidence preservation and documentation

---

## Tools Used

| Tool / Technique | Purpose |
|---|---|
| WhatWeb | Web technology fingerprinting |
| Gobuster | Directory/resource enumeration |
| cURL | HTTP request and response analysis |
| Browser / Web testing | Application interaction and validation |
| John the Ripper / password-recovery tooling | PDF password recovery |
| ExifTool | PDF metadata analysis |
| pdftotext | PDF content extraction |
| qpdf | PDF encryption/decryption analysis |

---

## Milestone Summary

### M1 — Initial Access

**Objective:** Validate the weakness that enabled access to restricted functionality.

The assessment included reconnaissance, technology identification, header analysis, directory enumeration, `robots.txt` review, username enumeration, input-handling testing, SQL injection validation, and restricted-area access validation.

**Public documentation:** `M1-Initial-Access/README.md`

---

### M2 — Data Extraction

**Objective:** Assess the security of three protected patient-report PDFs.

The documented workflow covers collection, protection analysis, password/hash recovery, decryption, and validation of the recovered documents.

The actual patient documents and password material are **not published** in this public repository.

**Public documentation:** `M2-Data-Extraction/README.md`

---

### M3 — Critical Data Exposure

**Objective:** Investigate whether the compromise exposed additional sensitive information.

The investigation path progressed from recovered material and metadata to an exposed legacy resource and database backup.

The public repository describes the exposure and its security impact without publishing the underlying employee, salary, shareholder, or database records.

**Public documentation:** `M3-Critical-Data-Exposure/README.md`

---

## Findings Summary

| ID | Finding | Severity | Demonstrated Impact |
|---|---|---|---|
| F-01 | Authentication / SQL injection weakness | Critical | Unauthorized access to restricted patient-report functionality |
| F-02 | Recoverable PDF password protection | High | Protected reports could be accessed after password recovery |
| F-03 | Exposed database backup | Critical | Sensitive personnel and corporate information was accessible |

> Detailed formal risk treatment and remediation belong in the final penetration-testing report.

---

## Public vs. Private Evidence

This portfolio repository intentionally contains only material suitable for public viewing.

### Included
- Project overview
- Scope and methodology
- Milestone documentation
- Tooling
- Findings summary
- Sanitized project structure
- Security lessons and assessment context

### Excluded
- Patient report files
- Decrypted patient documents
- Database dumps
- Salary records
- Shareholder records
- Passwords/hashes
- Other sensitive raw evidence
- Final M4 penetration-testing report

The complete evidence package remains separate for academic submission.

---

## Repository Structure

```text
.
├── M1-Initial-Access/
│   └── README.md
├── M2-Data-Extraction/
│   └── README.md
├── M3-Critical-Data-Exposure/
│   └── README.md
├── M4-Final-Report/
│   └── README.md
└── README.md
```

---

## Assessment Status

| Milestone | Status |
|---|---|
| M1 — Initial Access | Completed |
| M2 — Data Extraction | Completed |
| M3 — Critical Data Exposure | Completed |
| M4 — Final Report | Maintained separately |

---

## Lessons Demonstrated

This project demonstrates practical skills in:

- Black-box web application assessment
- Reconnaissance and enumeration
- Authentication and input validation testing
- SQL injection identification and validation
- Protected-document security assessment
- Password recovery analysis
- Digital artifact and metadata analysis
- Exposure-path investigation
- Sensitive-data impact assessment
- Penetration-testing evidence organization

---

## Responsible Use

This repository is provided for cybersecurity education and portfolio purposes.

The techniques described here must only be used against systems for which explicit authorization has been provided.

---

## Disclaimer

This work was performed within the authorized Networkwalks B083 educational environment. It should not be interpreted as a production security assessment of any real organization.
