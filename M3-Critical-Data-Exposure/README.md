# M3 — Critical Data Exposure

## Objective

Investigate whether material obtained during the assessment could lead to further exposure of sensitive information.

## Investigation Path

```text
Initial Access
      ↓
Patient Reports
      ↓
PDF Content / Metadata
      ↓
Legacy / Exposed Resource
      ↓
Database Backup
      ↓
Sensitive Records
```

## Assessment Activities

- PDF metadata analysis
- PDF content review
- Investigation of relevant clues
- Legacy resource validation
- Exposed-backup discovery and validation
- Impact assessment of exposed database information

## Impact

The assessment demonstrated exposure affecting sensitive personnel and corporate information, including staff, salary, and shareholder-related records within the training environment.

The actual records and database dump are intentionally excluded from this public repository.

## Key Security Lesson

Legacy files, backups, and forgotten web directories can create severe secondary exposure after an initial compromise. Production systems should prevent direct web access to backup artifacts and regularly review old resources.
