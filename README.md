🚀 Monitoring Project

Monitor SQL Server with Prometheus, Grafana, and SQL Exporter.

🧩 Stack

SQL Server – Your database

SQL Exporter – SQL metrics to Prometheus

Prometheus – Metrics collection & storage

Grafana – Dashboards & visualization

⚡ Quick Start
git clone <your-repo-url>
cd monitoring-project
docker compose up -d

Access services:

Grafana: http://localhost:3000
 (admin / admin123)

Prometheus: http://localhost:9090

Stop everything:

docker compose down
📌 Notes

SQL Exporter config → sql_exporter/sql_exporter.yml

Prometheus config → prometheus/prometheus.yml

Ensure Docker is running & ports 1433, 9399, 9090, 3000 are free
