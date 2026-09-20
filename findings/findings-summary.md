# Findings Summary

This file summarises the principal findings documented in the original university penetration-testing assessment.

## 1. MS17-010 / SMBv1 Exposure

**Original severity:** Critical

The Windows workstation was identified as Windows 7 SP1 with an SMBv1 implementation vulnerable to MS17-010. Controlled exploitation demonstrated the potential for remote code execution and highly privileged access.

### Recommended remediation

- Apply the relevant Microsoft security update
- Disable SMBv1 where it is not required
- Maintain a consistent patch-management process
- Review legacy operating systems and unsupported software

## 2. Weak SSH Credentials

**Original severity:** Critical

A dictionary-based password audit against the authorised SSH service recovered valid credentials for a server account. Those credentials were then used to establish an authenticated SSH session.

### Recommended remediation

- Enforce long, unique passwords
- Prevent reuse of weak or predictable passwords
- Reduce publicly exposed information that assists account enumeration
- Limit remote access to accounts that require it
- Consider stronger authentication controls for administrative access

## 3. Insecure File Permissions

**Original severity:** Critical

A writable server-hosted resource could be modified during the assessment. This allowed the exercise to demonstrate how weak permissions could be leveraged for further post-exploitation activity.

### Recommended remediation

- Apply least-privilege permissions to web-accessible files and directories
- Restrict write access to authorised users and processes
- Separate uploaded content from executable content
- Review permissions on shared directories and web-server paths

## Notes

Severity labels above preserve the classifications used in the original assessment. The portfolio presentation does not claim that a modern scoring framework such as CVSS was used at the time.
