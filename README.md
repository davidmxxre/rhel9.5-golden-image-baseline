# RHEL 9.5 Golden Image Baseline

## Summary
Built a hardened RHEL 9.5 golden image to establish a secure, repeatable baseline aligned with DISA STIG requirements

## Scope
This baseline includes:
- OS integrity enforcement
- System identity standardization
- Secure environment configuration
- Centralized time synchronization

## Key Controls
- Enforced system-wide UMASK (027)
- Disabled unused filesystems (cramfs, squashfs, udf)
- Restricted time synchronization sources

## Outcome
- Reduced attack surface
- Standardized system deployment baseline
- Improved  audit and compliance readiness

## Validation
All configurations were verified using system commands and service checks (see /evidence).

## Structure
- `/configs` -> applied system configurations
- `/docs` -> design decisions
- `/evidence` -> validation outputs
