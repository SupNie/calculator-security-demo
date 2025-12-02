# Security Scanning

## Overview
This repository uses three types of security scanning:


### SAST (Static Analysis with CodeQL)
- Scans source code for vulnerabilities
- Runs on push to main branch
- Checks for: [Code Analysis]
- Artifacts: See GitHub Security tab

### SCA (Dependency Check)
- Scans Python packages for known CVEs
- Runs on push to main branch
- Checks for: [false-postive, false-negative]
- Artifacts: sca-reports

### DAST (Live Application with ZAP)
- Tests running application for vulnerabilities
- Runs on push to main branch
- Checks for: [ZAP]
- Artifacts: zap-baseline-reports, zap-fullscan-reports

## Understanding Results
[

    FAIL-NEW: 0	FAIL-INPROG: 0	WARN-NEW: 7	WARN-INPROG: 0	INFO: 0	IGNORE: 0	PASS: 140
    
    http://localhost:5000/ (200 OK)
	http://localhost:5000/robots.txt (404 NOT FOUND)
	http://localhost:5000/sitemap.xml (404 NOT FOUND)
	http://localhost:5000 (200 OK)
	http://localhost:5000/favicon.ico (404 NOT FOUND)]

## Reporting Vulnerabilities
Please go to https://localhost:5000