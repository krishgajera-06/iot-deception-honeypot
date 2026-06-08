# Project Structure

## Main Components

### Cowrie Honeypot
Simulates a vulnerable SSH-based IoT device and captures attacker interactions.

### Promtail
Collects Cowrie logs and forwards them to Loki.

### Loki
Stores and indexes logs for analysis.

### Grafana
Visualizes attack activity through dashboards.

## Folder Structure

iot-deception-honeypot/
├── cowrie/
├── docs/
├── screenshots/
├── dashboard/
├── reports/
├── docker-compose.yml
├── promtail-config.yaml
└── README.md

## Data Flow

Attacker
↓
Cowrie Honeypot
↓
cowrie.json
↓
Promtail
↓
Loki
↓
Grafana Dashboard