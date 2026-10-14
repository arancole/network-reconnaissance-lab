
## Lab 1: Localhost TCP Reconnaissance

### Objective
Practice basic network reconnaissance using Nmap against the local Kali system.

### Scope
- Target: 127.0.0.1 (localhost)
- Tool: Nmap 7.99
- Scan type: TCP port scan with service-version detection
- Command: `nmap -sV 127.0.0.1`
- Ports examined: Nmap's default 1,000 most common TCP ports

### Results
- Host status: Up
- Open TCP ports detected: 0
- Closed TCP ports: 1,000
- Scan completed successfully.

### Analysis
The target responded to the scan. All 1,000 TCP ports examined were reported closed, indicating that no services were listening on those ports at the time of testing.

This result applies only to the scanned TCP ports. It does not establish that every port is closed or that the system has no security vulnerabilities.

### Security Recommendations
- Keep unnecessary network services disabled.
- Review listening services periodically.
- Restrict access to services that must be exposed.
- Repeat testing after significant system or configuration changes.

### Evidence
Raw scan output: `scans/localhost-scan.txt`

### Lessons Learned
Practiced Nmap service detection, saved scan evidence, and interpreted the difference between a closed port and an open port.
