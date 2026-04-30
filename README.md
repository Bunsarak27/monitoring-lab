This repository contains a local monitoring lab for the CyberLab monitoring project. 
It uses Docker Compose to start Prometheus, Grafana, and Blackbox Exporter for early testing. 

How to run locally: clone, enter folder, run compose, open URLs.
Default ports: Grafana 3300, Prometheus 9090, Blackbox 9115. 

## Prerequisites

Make sure you have installed:
- Docker
- Docker Compose

## Run locally

Clone the repository and start the containers:

```bash
git clone https://github.com/Bunsarak27/monitoring-lab.git
cd monitoring-lab
docker compose up -d
```

To stop the stack:

```bash
docker compose down
```

To check logs:

```bash
docker compose logs -f prometheus
docker compose logs -f grafana
docker compose logs -f blackbox
```

## Services

After starting the stack, open:

- Grafana: http://localhost:3300
- Prometheus: http://localhost:9090
- Blackbox Exporter: http://localhost:9115

## Default Grafana login

- Username: `admin`
- Password: `admin`
