# 🔎 Digital Evidence Forensics

A practical **Digital Forensics Investigation Project** demonstrating the end-to-end handling of controlled synthetic digital evidence.

## 📌 Project Overview

This project demonstrates a structured forensic workflow:

```text
Case Information
↓
Evidence Inventory
↓
Chain of Custody
↓
Evidence Acquisition
↓
SHA-256 Hashing
↓
Hash Verification
↓
File-System Examination
↓
Timeline Analysis
↓
Forensic Findings
↓
Final Forensic Report
```
## Evidence Set

This project uses controlled synthetic laboratory evidence.

| Evidence ID | File | Type | Size |
|---|---|---|---:|
| E001 | case-note.txt | ASCII text | 33 bytes |
| E002 | evidence-note.txt | ASCII text | 40 bytes |
| E003 | evidence-sample.tar.gz | gzip archive | 229 bytes |

## Evidence Integrity

SHA-256 verification was performed on all three evidence items.

```text
E001  case-note.txt
E002  evidence-note.txt
E003  evidence-sample.tar.gz

Verification Result: PASS
```

Verification command:

```bash
sha256sum -c 04-Hash-Verification/evidence-sha256.txt
```

## Forensic Tools

- Termux
- Git
- sha256sum
- stat
- file
- tar
- Markdown

## Investigation Results

- Evidence identification
- Evidence hashing
- Hash integrity verification
- File metadata examination
- File type identification
- Archive examination
- Timeline construction
- Findings documentation
- Final forensic reporting
## Timeline

| Time (IST) | Artifact |
|---|---|
| 15:03:28 | case-note.txt |
| 15:03:42 | evidence-note.txt |
| 15:05:01 | evidence-sample.tar.gz |

These timestamps belong to the controlled synthetic laboratory dataset.

## Documentation

| Phase | Directory |
|---|---|
| Case Information | `01-Case-Information/` |
| Chain of Custody | `02-Chain-of-Custody/` |
| Evidence Acquisition | `03-Evidence-Acquisition/` |
| Hash Verification | `04-Hash-Verification/` |
| Forensic Analysis | `05-Forensic-Analysis/` |
| Timeline | `06-Timeline/` |
| Findings | `07-Findings/` |
| Screenshots | `08-Screenshots/` |
| Final Report | `09-Final-Report/` |

## Final Report

Complete forensic examination report:

`09-Final-Report/final-report.md`
## Disclaimer

This is a controlled synthetic training and internship portfolio project.

No real user data, third-party data, or unauthorized systems were examined.

The documented timestamps and findings are limited to the supplied synthetic evidence dataset.

## Project Purpose

This project demonstrates practical digital forensic evidence handling, integrity verification, examination, timeline analysis and forensic reporting.

## Project Status

**Investigation Completed**

**Case ID:** DFIR-01-2026

**Report Version:** 1.0

**Classification:** Synthetic Training / Internship Portfolio Project
