# Design Overview - Golden Image Baseline

## Objective
Create a secure, minimal, and standardized RHEL 9.5 image for enterprise deployment.

------

## Operating System Integrity

### Minimal Installation
A minimal package set was used to reduce the attack surface and limit unnecessary services.

### Filesystem Hardening
Unused Filesystems were disabled
- cramfs
- squashfs
- udf

**Reason:**
Required for legal notification and STIG compliance

---

## Time Synchronization

### Chrony Configuration
System configured to use controlled NTP sources.

**Reason:**
Accurate time is critical for:
- Log correlation
- SIEM ingestion
- Incident response timeliness
