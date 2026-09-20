# Methodology

## Assessment Type

The original exercise was conducted as a **black-box penetration test** in an authorised university lab.

The objective was to assess a simulated SME environment with no prior knowledge of the target infrastructure, identify security weaknesses, demonstrate their potential impact in a controlled manner, and recommend remediation.

## Workflow

### Reconnaissance and Enumeration

- Discover hosts on the assessment network
- Configure the testing system for the target subnet
- Enumerate target services and operating systems
- Run vulnerability-oriented Nmap scans

### Vulnerability Validation

- Investigate identified vulnerabilities
- Select appropriate tools and modules
- Attempt controlled exploitation
- Troubleshoot failed execution where necessary

### Credential Security Testing

- Identify a valid account from available lab information
- Perform authorised dictionary-based SSH password testing
- Validate discovered credentials through SSH access

### Post-Exploitation

- Enumerate users and system resources
- Assess file and directory permissions
- Test reverse-shell behaviour
- Audit password material with John the Ripper
- Demonstrate the effect of privileged access

### Reporting

The original report concluded with:

- Documented findings
- Severity classifications
- Technical impact
- Remediation recommendations

## Scope and Ethics

All activity documented in this repository was performed against systems provided for the university assessment. The repository is intended to demonstrate methodology and learning, not to provide instructions for unauthorised access.
