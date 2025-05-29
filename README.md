# Task-3
# Full Vulnerability Scan Using Nessus Essentials

## Project Overview
This project involves performing a basic vulnerability scan on a Windows 11 system using Nessus Essentials. The scan identifies security weaknesses, providing insight into potential risks and possible mitigations.

## Deliverables
- **Full Vulnerability Scan Report** containing identified security issues.
- **Scan Results screenshot**
- **This readme file**

## Critical Vulnerabilities Identified
### 1. SMB Signing Not Required
- **Description**: The remote SMB server does not enforce signing, allowing an unauthenticated attacker to conduct man-in-the-middle attacks.
- **CVSS Scores**:
  - CVSS v3.0 Base Score: **5.3**
  
- **Mitigation**: Enforce message signing in the host configuration.
  - On Windows: Enable `Microsoft network server: Digitally sign communications (always)`.
  

### 2. SSL Certificate Cannot Be Trusted
- **Description**: The server's SSL certificate cannot be trusted due to missing intermediate certificates, invalid certificate dates, or unverified signatures.
- **CVSS Scores**:
  - CVSS v3.0 Base Score: **6.5**
  
- **Mitigation**: Obtain a valid SSL certificate from a recognized certificate authority.

## System Information
- **Hostname**: MAKBOOK007
- **IP Address**: 192.168.1.6
- **Operating System**: Windows 11

## Summary
This vulnerability scan highlights security risks on the system, offering solutions to improve network protection and certificate authenticity.
