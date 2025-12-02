# Security Scan Analysis - [2/12/2025]

## DAST Results (ZAP Baseline)
- Total URLs scanned: 10
- PASS: 140 checks
- WARN-NEW: 7 warnings
- FAIL-NEW: 0 failures

### Warning Summary
[1. Missing Anti-clickjacking Header [10020] x 2 , 2. X-Content-Type-Options Header Missing [10021] x 2 , 3. Server Leaks Version Information via "Server" HTTP Response Header Field [10036] x 5 , 
4. Content Security Policy (CSP) Header Not Set [10038] x 5, 5.Permissions Policy Header Not Set [10063] x 5, 6. HTTP Only Site [10106] x 1 , 7. Insufficient Site Isolation Against Spectre Vulnerability [90004] x 6
]

## SCA Results (Dependency Check)
- High severity: 3
- Medium severity: 4
- Low severity: 1

### Vulnerable Packages
[Werkzeug (pip)]

## SAST Results (CodeQL)
- Total issues: 1
- By type: [Flask app is run in debug mode]

## Recommendations
[Patch High-Severity Vulnerabilities from SCA, Remediate Security Header Issues Detected by DAST]