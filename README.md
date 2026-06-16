# Linux Forensic File Recovery and Artifact Analysis

## Overview

This project documents a Linux forensic investigation focused on recovering hidden, deleted, and camouflaged files from a Linux system. The investigation involved identifying concealed artifacts, recovering deleted image files through file carving techniques, extracting metadata from recovered evidence, and validating evidence integrity using MD5 hash analysis.

The objective was to demonstrate core digital forensic techniques commonly used during incident response and forensic examinations to locate, recover, and analyze potentially malicious or hidden data residing on a Linux system.

---

## Objectives

- Identify camouflaged files disguised as legitimate system artifacts
- Locate hidden files across the Linux filesystem
- Recover deleted files using forensic recovery tools
- Extract and analyze metadata from recovered artifacts
- Validate recovered evidence using MD5 hash verification
- Document forensic findings and investigative methodology

---

## Skills Demonstrated

### Linux Forensics
- Linux filesystem analysis
- Hidden file discovery
- Artifact identification
- Evidence validation

### File Recovery
- File carving
- Deleted file recovery
- Metadata extraction
- EXIF analysis

### Digital Forensics
- Chain of evidence documentation
- Hash verification
- Artifact correlation
- Investigative reporting

---

## Tools Utilized

| Tool | Purpose |
|--------|---------|
| Linux Command Line | File discovery and analysis |
| Foremost | File carving and recovery |
| Scalpel | Recovery of deleted files |
| Exiv2 | Metadata extraction |
| MD5SUM | Hash verification |
| Bash Utilities | File identification and validation |

---

## Investigation Summary

The investigation identified:

### Camouflaged Files
- `eruces.log`
- `sha1337sum`

### Hidden Files
- Multiple hidden artifacts discovered in:
  - `/root`
  - `/var/opt/help`
  - `/usr/share/mosaics`

### Deleted Artifacts
- Recovery of deleted image files using forensic carving techniques
- Metadata extraction from recovered files
- Validation of recovered evidence through MD5 hashing

---

## Repository Structure

```text
linux-forensic-file-recovery/

├── README.md
├── Executive-Summary.md
├── Findings.md
├── Analysis.md
├── Evidence.md
├── Recommendations.md
│
└── Assets/
    └── screenshots/
```

---

## Key Findings

- Hidden files were successfully identified across multiple directories.
- Camouflaged files were discovered masquerading as legitimate system files.
- Deleted image artifacts were recovered through forensic carving methods.
- Metadata analysis revealed embedded forensic flags.
- MD5 hash verification confirmed artifact integrity.
