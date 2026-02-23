# 🚀 Monitoring Project
**Monitor SQL Server** with **Prometheus**, **Grafana**, and **SQL Exporter**.

## 🧩 Stack
- **SQL Server** – Your database  
- **SQL Exporter** – SQL metrics to Prometheus  
- **Prometheus** – Metrics collection & storage  
- **Grafana** – Dashboards & visualization  

## ⚡ Quick Start
```bash
git clone https://github.com/samawael7/docker-monitoring-project.git
cd monitoring-project
docker compose up -d
```

> Wait ~30 seconds for SQL Server to become healthy.

## 🌐 Access
| Service | URL | Login |
|---|---|---|
| Grafana | http://localhost:3000 | admin / admin123 |
| Prometheus | http://localhost:9090 | — |
| SQL Exporter | http://localhost:9399/metrics | — |

## 📈 Metrics
| Metric | Description |
|---|---|
| `mssql_up` | Server availability |
| `mssql_connections` | Active connections |
| `mssql_cpu_usage_percent` | CPU usage % |
| `mssql_memory_usage_bytes` | Memory used |
| `mssql_batch_requests_total` | Batch requests/sec |

## 🏗️ Architecture
Prometheus ──► SQL Exporter ──► SQL Server
│
▼
Grafana

## 🛠️ Tech Stack
**Docker** · **Docker Compose** · **SQL Server 2022** · **Prometheus** · **Grafana** · **SQL Exporter**
