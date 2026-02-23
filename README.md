🐳 Docker Monitoring Stack
A production-ready monitoring stack using Docker Compose, featuring Prometheus, Grafana, and Microsoft SQL Server with custom metrics collection via SQL Exporter.

📊 Dashboard:

Grafana dashboard showing real-time SQL Server metrics including CPU usage, memory, connections, and batch requests.

🏗️ Architecture
┌─────────────┐     scrapes     ┌──────────────┐     queries     ┌─────────────┐
│  Prometheus │ ──────────────► │ SQL Exporter │ ──────────────► │ SQL Server  │
└─────────────┘                 └──────────────┘                 └─────────────┘
       │
       │ data source
       ▼
┌─────────────┐
│   Grafana   │
└─────────────┘
ServiceImagePortSQL Server 2022mcr.microsoft.com/mssql/server:2022-latest1433SQL Exporterburningalchemist/sql_exporter:latest9399Prometheusprom/prometheus:latest9090Grafanagrafana/grafana:latest3000
