# Evidence

## Evidence Collection Overview

Evidence was collected through a structured Linux forensic examination focused on identifying hidden files, camouflaged artifacts, deleted files, metadata, and integrity verification information. The investigation utilized Linux forensic tools and command-line utilities to locate, recover, analyze, and validate evidence discovered throughout the system.

All screenshots associated with the investigation are stored within the repository's `Assets/screenshots` directory.

---

# Evidence Inventory

## Evidence 01 – Camouflaged File Discovery

**Screenshot:** `01-camouflaged-file-eruces-log.png`

### Description
A suspicious file named `eruces.log` was identified during filesystem analysis. The filename appeared intentionally modified to resemble a legitimate log file while concealing its true purpose.

### Significance
The file demonstrates a common anti-forensic technique where filenames are crafted to blend into normal system activity and evade detection.

---

## Evidence 02 – Additional Camouflaged File

**Screenshot:** `02-camouflaged-file-sha1337sum.png`

### Description
A second suspicious file named `sha1337sum` was identified. The filename closely resembles the legitimate Linux hashing utility `sha1sum`.

### Significance
The naming convention suggests an attempt to disguise the artifact as a trusted system utility.

---

## Evidence 03 – Hidden File Discovery in Root Directory

**Screenshot:** `03-hidden-file-root.png`

### Description
Hidden files were discovered within the `/root` directory during filesystem analysis.

### Significance
Hidden files located within privileged user directories may contain sensitive information or unauthorized artifacts.

---

## Evidence 04 – Hidden File Discovery in /var/opt/help

**Screenshot:** `04-hidden-file-var-opt-help.png`

### Description
Additional hidden files were identified within the `/var/opt/help` directory.

### Significance
This demonstrates how hidden files can be distributed across multiple filesystem locations to reduce visibility.

---

## Evidence 05 – Hidden File Discovery in /usr/share/mosaics

**Screenshot:** `05-hidden-file-usr-share-mosaics.png`

### Description
Hidden artifacts were located within the `/usr/share/mosaics` directory.

### Significance
Attackers frequently leverage uncommon directories to conceal artifacts and avoid routine administrative review.

---

## Evidence 06 – File Recovery Operation

**Screenshot:** `06-file-recovery-process.png`

### Description
Forensic recovery tools were used to identify and recover deleted files from the Linux system.

### Significance
This process demonstrates the ability to recover evidence that persists after deletion attempts.

---

## Evidence 07 – Recovered Image Artifact

**Screenshot:** `07-recovered-image-1.png`

### Description
A deleted image file was successfully recovered through forensic carving techniques.

### Significance
Recovered image files may provide valuable investigative context regarding user activity or system events.

---

## Evidence 08 – Additional Recovered Image Artifact

**Screenshot:** `08-recovered-image-2.png`

### Description
A second deleted image file was recovered from the system.

### Significance
Multiple recovered artifacts indicate that deleted evidence remained accessible within the filesystem.

---

## Evidence 09 – Additional Recovered Image Artifact

**Screenshot:** `09-recovered-image-3.png`

### Description
Another deleted image artifact was successfully recovered.

### Significance
The recovery process demonstrates the effectiveness of file carving techniques during forensic investigations.

---

## Evidence 10 – Additional Recovered Image Artifact

**Screenshot:** `10-recovered-image-4.png`

### Description
A fourth deleted image file was recovered during analysis.

### Significance
The artifact contributed to the overall evidence set recovered from the system.

---

## Evidence 11 – Metadata Analysis

**Screenshot:** `11-exiv2-metadata-analysis.png`

### Description
Metadata extraction was performed using Exiv2 to analyze attributes associated with recovered files.

### Evidence Collected

- File metadata
- Embedded attributes
- Creation and modification information
- Application-specific details

### Significance

Metadata provides contextual information that supports artifact validation and timeline reconstruction.

---

## Evidence 12 – MD5 Hash Verification

**Screenshot:** `12-md5-verification.png`

### Description

MD5 hashing was performed against recovered artifacts to verify evidence integrity.

### Evidence Collected

- MD5 hash values
- File integrity validation results

### Significance

Hash verification confirms that evidence remains unchanged throughout the investigation and supports forensic reliability.

---

# Evidence Summary

The investigation produced evidence in the following categories:

| Evidence Type | Quantity |
|--------------|----------|
| Camouflaged Files | 2 |
| Hidden File Discoveries | 3 |
| Deleted File Recoveries | 5 |
| Metadata Analysis Artifacts | 1 |
| Integrity Verification Results | 1 |

---

# Chain of Custody Considerations

All evidence was collected through forensic analysis techniques designed to preserve data integrity. Recovered artifacts were validated through cryptographic hashing, and investigative findings were documented through screenshots and analysis notes.

The evidence collected supports the conclusions documented throughout this investigation and demonstrates the effectiveness of Linux forensic methodologies in identifying concealed and deleted artifacts.
