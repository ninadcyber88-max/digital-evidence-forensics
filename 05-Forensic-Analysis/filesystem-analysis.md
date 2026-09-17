# File System Forensic Analysis

## Case ID

DFIR-01-2026

## Evidence Examined

`case-note.txt`

## Examination Tool

Termux `stat` utility

## File Metadata

| Field | Value |
|---|---|
| File Name | case-note.txt |
| Size | 33 bytes |
| File Type | Regular file |
| Permissions | 0600 |
| Links | 1 |
| UID | 10565 |
| GID | 10565 |
| Access Time | 2026-09-17 15:03:28 +0530 |
| Modify Time | 2026-09-17 15:03:28 +0530 |
| Change Time | 2026-09-17 15:03:28 +0530 |
| Birth Time | Not available |

## Observation

The examined file is a regular 33-byte file with permissions
set to `0600`.

The Access, Modify and Change timestamps are recorded at
approximately the same timestamp.

## Forensic Interpretation

The timestamps provide file-system metadata that can be used
for timeline correlation.

The timestamps alone do not establish who created, accessed,
or modified the file.

Additional independent artifacts are required for correlation.

## Evidence Integrity

SHA-256:

`b82145e892f746782d7c68efa15005476a0740474529977d07d2f80eaf5b147e`

## Status

Examined
