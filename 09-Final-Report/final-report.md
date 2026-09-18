# DIGITAL FORENSIC INVESTIGATION REPORT

## Case ID

DFIR-01-2026

## Report Type

Digital Evidence Forensic Examination Report

## Examination Environment

Authorized Synthetic Digital Forensics Laboratory

---

## 1. Executive Summary

This report documents the forensic examination of a controlled
synthetic digital evidence dataset.

The examination included evidence identification, SHA-256 hashing,
hash verification, file metadata examination, file type
identification, archive examination, timeline correlation and
forensic reporting.

The examined evidence consisted of:

- case-note.txt
- evidence-note.txt
- evidence-sample.tar.gz

All three evidence items successfully passed SHA-256 integrity
verification.

---

## 2. Investigation Objectives

1. Identify the supplied digital evidence.
2. Preserve evidence integrity using cryptographic hashing.
3. Verify evidence using SHA-256.
4. Examine file-system metadata.
5. Identify file types.
6. Examine archive contents.
7. Establish a basic forensic timeline.
8. Document forensic findings.
9. Produce a reproducible forensic report.

---

## 3. Evidence Inventory

| Evidence ID | File Name | Size | Type |
|---|---|---:|---|
| E001 | case-note.txt | 33 bytes | ASCII text |
| E002 | evidence-note.txt | 40 bytes | ASCII text |
| E003 | evidence-sample.tar.gz | 229 bytes | gzip compressed data |

---

## 4. Evidence Integrity

| Evidence ID | SHA-256 | Verification |
|---|---|---|
| E001 | b82145e892f746782d7c68efa15005476a0740474529977d07d2f80eaf5b147e | PASS |
| E002 | 62350214b23ab15ddd8f71926303430ceef54328a1e153785f976dceb1b88b3f | PASS |
| E003 | 9e2d08407ad83ae1f346c6eedda01c9b59a3321485a89b93bfb65632780aa7dd | PASS |

Verification command:

sha256sum -c 04-Hash-Verification/evidence-sha256.txt

Result:

case-note.txt: OK
evidence-note.txt: OK
evidence-sample.tar.gz: OK

---

## 5. File-System Examination

The stat utility was used to examine file-system metadata.

### E001 — case-note.txt

- Size: 33 bytes
- Permissions: 0600
- Access: 2026-09-17 15:03:28 +0530
- Modify: 2026-09-17 15:03:28 +0530
- Change: 2026-09-17 15:03:28 +0530
- Birth: Not available

### E002 — evidence-note.txt

- Size: 40 bytes
- Permissions: 0600
- Access: 2026-09-17 15:03:42 +0530
- Modify: 2026-09-17 15:03:42 +0530
- Change: 2026-09-17 15:03:42 +0530
- Birth: Not available

### E003 — evidence-sample.tar.gz

- Size: 229 bytes
- Permissions: 0600
- Access: 2026-09-17 15:05:01 +0530
- Modify: 2026-09-17 15:05:01 +0530
- Change: 2026-09-17 15:05:01 +0530
- Birth: Not available

---

## 6. File Type Examination

The file utility identified:

- case-note.txt as ASCII text.
- evidence-note.txt as ASCII text.
- evidence-sample.tar.gz as gzip compressed data.

---

## 7. Archive Examination

The archive was examined using:

tar -tzf evidence-sample.tar.gz

Archive contents:

- case-note.txt
- evidence-note.txt

---

## 8. Forensic Timeline

| Time (IST) | Artifact | Observation |
|---|---|---|
| 15:03:28 | case-note.txt | File-system timestamp observed |
| 15:03:42 | evidence-note.txt | File-system timestamp observed |
| 15:05:01 | evidence-sample.tar.gz | File-system timestamp observed |

The available timestamps establish a chronological sequence
within the examined synthetic dataset.

---

## 9. Findings

### F-001 — Evidence Identification

Three synthetic evidence artifacts were successfully identified
and classified.

### F-002 — Evidence Integrity

All three evidence artifacts successfully passed SHA-256
verification.

### F-003 — Archive Contents

The gzip archive was successfully examined and its contents
were identified.

### F-004 — File-System Metadata

File size, permissions and MAC timestamps were documented.

### F-005 — Timeline

A basic chronological sequence was established from the available
file-system timestamps.

---

## 10. Forensic Assessment

The examination demonstrated a controlled digital-forensic
workflow covering evidence identification, hashing, verification,
metadata examination, archive examination, timeline creation,
findings and reporting.

The integrity verification checks passed.

No conclusion regarding a real-world security incident,
unauthorized access, user identity or user intent is made from
this synthetic dataset alone.

---

## 11. Limitations

1. The dataset is synthetic laboratory evidence.
2. No real user or third-party data was examined.
3. File-system timestamps alone cannot establish attribution.
4. The examination is limited to the artifacts listed in this report.
5. Additional independent forensic artifacts would be required
   for a broader investigation.

---

## 12. Tools Used

- Termux
- Git
- sha256sum
- stat
- file
- tar
- Markdown

---

## 13. Reproducibility

The examination commands and forensic documentation are stored
within the project repository.

The workflow can be reproduced against the same synthetic
dataset using the documented commands.

---

## 14. Conclusion

The controlled synthetic evidence set was successfully examined.

Evidence identification, SHA-256 integrity verification,
file-system metadata examination, file-type identification,
archive examination, timeline creation and forensic findings
documentation were completed.

## Investigation Status

COMPLETED

## Case Classification

Synthetic Training / Internship Portfolio Project

## Report Version

1.0

---

Prepared for: Digital Forensics Internship Portfolio

Case ID: DFIR-01-2026
