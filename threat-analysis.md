# Threat Analysis Report

## Overview
The IoT Deception Honeypot captures attacker activities through the Cowrie SSH honeypot and forwards logs for monitoring and analysis.

## Observed Events
- SSH login attempts
- Command execution
- Session creation
- Session termination

## Sample Commands Captured
- ls
- pwd
- whoami
- wget malware.sh

## Log Collection Pipeline
Cowrie → Promtail → Loki → Grafana

## Security Benefits
- Attacker behavior analysis
- Threat monitoring
- Incident investigation
- Security awareness

## Conclusion
The system successfully captures and visualizes attacker activity in a controlled environment.