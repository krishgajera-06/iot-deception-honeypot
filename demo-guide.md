# IoT Deception Honeypot Demo Guide

## Step 1: Start Containers

sudo docker compose up -d

## Step 2: Verify Services

sudo docker ps

Services:
- Cowrie
- Grafana
- Loki
- Promtail

## Step 3: Simulate Attack

ssh root@<IP> -p 2222

Commands:
ls
pwd
whoami

## Step 4: Verify Logs

tail -f cowrie/var/log/cowrie/cowrie.json

## Step 5: Open Grafana

http://localhost:3000

## Step 6: View Dashboard

- Live Attack Logs
- SSH Login Attempts
- Attacker Commands
- Attack Timeline

## Expected Outcome

The attack activity should be captured by Cowrie, forwarded through Promtail and Loki, and visualized in Grafana.